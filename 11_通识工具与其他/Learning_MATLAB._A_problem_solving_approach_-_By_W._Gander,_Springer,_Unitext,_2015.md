

<!-- === Source: MinerU_markdown_Learning_MATLAB._A_problem_solving_approach_-_By_W._Gander,_Springer,_Unitext,_2015_1_2122707067558010887.md (Page 1) === -->

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/83880a289ed09d416d8bc7c9d2711a4c7ece4488a924d87a0b583ec21e54da9d.jpg)


Learning MATLAB 

A Problem Solving Approach 

123 

# UNITEXT - La Matematica per il 3+2

Volume 95 

Editor-in-chief 

A. Quarteroni 

Series editors 

L. Ambrosio 

P. Biscari 

C. Ciliberto 

M. Ledoux 

W.J. Runggaldier 

More information about this series at http://www.springer.com/series/5418 

Walter Gander 

# Learning MATLAB

A Problem Solving Approach 

ISSN 2038-5722 

ISSN 2038-5757 (electronic) 

UNITEXT - La Matematica per il 3+2 

ISBN 978-3-319-25326-8 

ISBN 978-3-319-25327-5 (eBook) 

DOI 10.1007/978-3-319-25327-5 

Library of Congress Control Number: 2015953792 

Mathematics Subject Classification (2010): 65-XX 

Springer Cham Heidelberg New York Dordrecht London 

© Springer International Publishing Switzerland 2015 

This work is subject to copyright. All rights are reserved by the Publisher, whether the whole or part of the material is concerned, specifically the rights of translation, reprinting, reuse of illustrations, recitation, broadcasting, reproduction on microfilms or in any other physical way, and transmission or information storage and retrieval, electronic adaptation, computer software, or by similar or dissimilar methodology now known or hereafter developed. 

The use of general descriptive names, registered names, trademarks, service marks, etc. in this publication does not imply, even in the absence of a specific statement, that such names are exempt from the relevant protective laws and regulations and therefore free for general use. 

The publisher, the authors and the editors are safe to assume that the advice and information in this book are believed to be true and accurate at the date of publication. Neither the publisher nor the authors or the editors give a warranty, express or implied, with respect to the material contained herein or for any errors or omissions that may have been made. 

Printed on acid-free paper 

Springer International Publishing AG Switzerland is part of Springer Science+Business Media (www.springer.com) 

# Acknowledgment

I would like to thank Dr. Karl Knop for his interest in this project, for proofreading several chapters and for solving problems and exercises. 

## Contents

1 Starting and Using MATLAB 1  
1.1 Organize Your Desktop. 1  
1.2 MATLAB Scripts and Functions 1  
1.2.1 MATLAB Script. 2  
1.2.2 MATLAB Function. 2  
1.3 The Windows Environment. 4  
1.4 The Linux Environment. 5  
1.5 Using GNU Octave. 6  
1.6 Documenting Results. 6  
1.7 MATLAB-Elements Used in This Chapter. 7  
1.8 Problems and Exercises. 9  
2 How a Computer Calculates. 11  
2.1 Finite Arithmetic. 11  
2.2 Rounding Errors. 12  
2.3 IEEE-Arithmetic. 13  
2.4 MATLAB-Elements Used in This Chapter. 15  
2.5 Problems. 16  
3 Plotting Functions and Curves. 17  
3.1 Plotting a Function. 17  
3.2 Plotting Curves. 20  
3.3 Plotting 3-d Curves. 20  
3.4 Surface and Mesh Plots. 21  
3.5 Contour Plots. 23  
3.6 MATLAB-Elements Used in This Chapter. 24  
3.7 Problems. 27  
4 Some Elementary Functions. 29  
4.1 Computing the Exponential Function. 30  
4.2 Computing sin and cos. 32  
4.3 Computing arctan. 32 

4.4 MATLAB-Elements Used in This Chapter 32
4.5 Problems 33

5 Computing with Multiple Precision 35
5.1 Computation of the Euler Number e 35
5.2 MATLAB-Elements Used in This Chapter 41
5.3 Problems 43

6 Solving Linear Equations 43
6.1 Gaussian Elimination and LU Decomposition 43
6.2 Elimination with Givens-Rotations 47
6.3 MATLAB-Elements Used in This Chapter 51
6.4 Problems 52

7 Recursion 57
7.1 Introduction 57
7.2 Laplace Expansion for Determinants 58
7.3 Hilbert Curves 60
7.4 Quicksort 63
7.5 MATLAB-Elements Used in This Chapter 64
7.6 Problems 65

8 Iteration and Nonlinear Equations 67
8.1 Bisection 67
8.2 Newton's Method 68
8.2.1 Algorithm of Heron 69
8.2.2 Fractal 69
8.3 Circular Billiard 70
8.4 MATLAB-Elements Used in This Chapter 74
8.5 Problems 75

9 Simulation 79
9.1 Event Simulation Using Random Numbers 79
9.2 Exhaustive Search 84
9.3 Differential Equations 87
9.3.1 Numerical Integrator ode45 88
9.3.2 Dog Attacking a Jogger 90
9.4 MATLAB-Elements Used in This Chapter 94
9.5 Problems 95

10 Solutions of Problems 99
10.1 Chapter 1: Starting 99
10.2 Chapter 2: How a Computer Calculates 99
10.3 Chapter 3: Plotting Functions and Curves 102
10.4 Chapter 4: Some Elementary Functions 105
10.5 Chapter 5: Computing with Multiple Precision 109
10.6 Chapter 6: Solving Linear Equations 113 

10.7 Chapter 7: Recursion ..... 123
10.8 Chapter 8: Iteration and Nonlinear Equations..... 128
10.9 Chapter 9: Simulation..... 138
Bibliography..... 149 

## How to Use This Book

The goal of this book is to teach MATLAB by examples, that is, by showing how to solve problems by designing an algorithm and implementing it in MATLAB. Cleve Moler developed MATLAB originally for teaching linear algebra. MATLAB is the acronym for “MATrix LABoratory.” Today MATLAB is a widely used computer language for technical computing. This book is not meant to cover the whole range of MATLAB. Rather it is an introduction to motivate the students to learn this programming language. 

The book is based on notes that have been written for a beginner course of 7 weeks with 3 hours of lectures and exercises per week, given at Qian Weichang College at Shanghai University in the fall of 2014. I am indebted to Ying Su for her help during that course and to Prof. Chuan-Qing Gu who invited me to lecture this course. 

Some examples were taken from the books [3], [4] and from the freely available online book of the M creator [8]. 

Most programs developed in this course can also be run using the public domain software GNU OCTAVE.<sup>1</sup> The OCTAVE language is quite similar to MATLAB so that programs are portable. 

Programming environments like MATLAB are very large systems. Getting familiar with the graphical user interface of MATLAB is for a beginner already a challenge. Chapter 1 gives a few hints how to get organized. 

It is not possible to get familiar with the whole MATLAB system in one semester, not even in several semesters! My approach is therefore based on learning by doing. Given a problem, one has to find a way to solve it using MATLAB. My experience is that the students memorize much better MATLAB commands and programming structures when they use it themselves. Therefore it is important to do the exercises before consulting Chap. 10 where all solutions are given. 

Several topics of the book are taken from my area of interest: Scientific Computing. The emphasis is, however, on programming. Showing how to compute some elementary functions using the four basic operations (Chap. 4) is just a nice programming exercise. Computations are mostly done with the usual IEEE arithmetic implemented in MATLAB. Chapter 2 describes the principles of this finite arithmetic. In Chap. 5 we use some of MATLAB’s integer arithmetic operations by working with unsigned integers. We do not make use of any of the many toolboxes of MATLAB, and especially we do not use Symbolic Math Toolbox Functions. It is important to tell the students the difference when computing with a computer algebra system versus using standard IEEE arithmetic. 

The other book which also teaches MATLAB but focuses more on scientific computing is [9]. 

Zürich, Switzerland 

Summer 2015 

Walter Gander 

# Some Historical Remarks on the Genesis of MATLAB

Linear Algebra, especially matrix algebra, is of the utmost importance for scientific calculations, as the solutions of many problems are constructed from fundamental operations in this field. Nonlinear problems are often solved iteratively in such a way that in each iteration step one has to solve a linear problem. These are essentially matrix operations, solving linear systems of equations and eigenvalue problems. This fact was recognized early on, so already in the 1960s, a program library for linear algebra was being constructed. At that time, scientific computing was performed exclusively in two programming languages, ALGOL 60 and FORTRAN. A series entitled “Handbook for Automatic Computation” was started by the Springer publishing company, so as to, one day, obtain a complete and reliable library of computer programs. The documentation language was defined to be ALGOL, as 

indeed, a correct ALGOL program is the abstractum of a computing process for which the necessary analyses have already been performed.<sup>2</sup> 

The first volume of the handbook consists of two parts: In the first part A, H. Rutishauser describes the reference language under the title “Description of ALGOL 60” [10], in the second part B “Translation of ALGOL 60,” the three authors Grau, Hill, and Langmaack [6] provide instructions on how to build a compiler. We have to be aware that in those times the computers were delivered with almost no software! 

The second volume of the handbook, edited by Wilkinson and Reinsch, appeared in 1971. Under the title of “Linear Algebra” [12], it contains various procedures to solve linear systems of equations and eigenvalue problems. The quality of this software is so good that the algorithms are still used today. 

Unfortunately, this series of handbooks was discontinued, as the fast development and distribution of information technology made any further coordination impossible. 

Because of the language barrier Europe—USA 

The code itself has to be in FORTRAN, which is the language for scientific programming in the United States.<sup>3</sup> 

the LINPACK [2] project was executed in 1970s at Argonne National Laboratory. LINPACK contains programs for the solution of fully occupied systems of linear equations. They were based on the procedures of the handbook, but had been renewed and systematically programmed in FORTRAN. This can be seen in the unified conventions for naming, portability, and machine independence (e.g., termination criteria), use of elementary operations by calling the BLAS (Basic linear Algebra Subprograms). The LINPACK Users Guide appeared in 1979. LINPACK is also the name of a benchmark for measuring performance of a computer in floating point operations. This benchmark used to consist of two parts: On the one hand, a given FORTRAN program had to be compiled and executed to solve a fully occupied 100 × 100 system of linear equations; on the other hand, a 1000 × 1000 system of linear equations had to be solved as fast as possible (using any adjusted program). This benchmark,<sup>4</sup> in a modified form, is now used every 6 months to determine the 500 most powerful computers in the world, so as to list them in the top 500 list, see http://www.top500.org. 

Also the eigenvalue procedures from [12] were translated into FORTRAN and are available under the name EISPACK [5], [11]. EISPACK and LINPACK were replaced a number of years ago by LAPACK [1]. The LINPACK, EISPACK, and LAPACK procedures (and many more) can be obtained electronically from the online software library NETLIB, see http://www.netlib.org. 

In the late 1970s, Cleve Moler developed the interactive program MATLAB (MATrix LABoratory), initially only to provide a simple calculation tool for lectures and exercises. The basis for this program, were programs from LINPACK and EISPACK. As efficiency considerations were not of great importance, only eight procedures from LINPACK and five from EISPACK for calculations with full matrices were included. MATLAB was not only established as a useful teaching aid, but also applied in contrary to the initial intention, in research and industry. The initially public domain M [7], written in FORTRAN was completely overworked, extended and made it into an efficient engineering tool by the company MathWorks.<sup>5</sup> It is now written in C. This philosophy in the development of MATLAB has led to a continuous writing of new function packages (so-called Toolboxes) for various fields of application. The user community has a discussion platform at MATLAB-Central http://www.mathworks.com/matlabcentral/?s_tid=gn_mlc_logo with a lot of useful information. 

# Chapter 1 Starting and Using MATLAB

## 1.1 Organize Your Desktop

Get rid ofnot necessary open windows on your computer. We need only two windows: one window for executing Matlab programs and a second one for writing programs. Make these windows as high and large as possible so that you can have a good overview of your programs and of the results. After starting Matlab it is a good idea to write the command format compact. This command eliminates blank lines and thus concentrates the output. 

Notice that Matlab programs are written as plain ASCII texts. You can use any editor to write them. If you use a Linux operating system then Emacs or vi are very good choices. 

## 1.2 MATLAB Scripts and Functions

You will write in Matlab your own programs and your own functions. It is important to distinguish between a program (or Matlab script) and a function. Matlab scripts are “main programs” and functions which you write can be used in them. The functions must be stored in the same directory where the script is which calls them. A Matlab-script is stored as a M-file (a file with the suffix .m) and is executed in the command window by typing its name without the suffix. 

Notice that you may want to store your programs in a special directory not necessarily the default directory where Matlab is called. For this you can use the command cd which is the abbreviation for “change directory”. For instance you may want to write your programs in a directory called c: LinearAlgebraProblems. Then after calling Matlab you can change directory in the command window with if you want to see what files are in that directory then use 

```txt
>> cd c:\LinearAlgebraProblems 
```

```txt
>> ls 
```

it will give you a list of all the files. 

## 1.2.1 MATLAB Script

Assume that you are given a linear equation 

$$
a x + b = 0
$$

and you would like to write a program to solve such equations. You could write the following text and save it as an M-file: 

```matlab
% solves the linear equation a*x+b=0 for x.
a=input('a=?')
b=input('b=?')
if a~=0,
    x=-b/a
elseif b==0,
    disp('any x is solution')
else
    disp('no solution')
end 
```

Now save this program under the name LinearScript.m and call this program in the Matlab command-window to solve the equation 3x 5 0 

```txt
>> LinearScript
a=?3
a =
    3
b=?5
b =
    5
x =
-1.6667 
```

## 1.2.2 MATLAB Function

A function can be called by different Matlab scripts and also by other functions. A function has input parameters and delivers results as output parameters. So for our linear equation the input parameters are the two coefficients a and b and the output parameter, the result, is the solution x. The function becomes 

## 1.2 Matlab Scripts and Functions

```matlab
function x=SolveLinear(a,b)
% SolveLinear solves the linear equation a*x+b=0
if a~=0,
    x=-b/a;
elseif b==0,
    error('any x is solution')
else
    error('no solution')
end 
```

Save this function under the name SolveLinear.m. Note that thefile name must be the same as the function name. Now in order to apply the function we can write in the Matlab window 

```txt
>> SolveLinear(3,5)
ans =
-1.6667 
```

Or we could type another Matlab script interactively in the Matlab window 

```matlab
>> b=1;
>> for a=-3:2
    a
    x=SolveLinear(a,b)
end
a =
-3
x =
0.3333
a =
-2
x =
0.5000
a =
-1
x =
1
a =
0
??? Error using ==> SolveLinear at 8
no solution 
```

the program stops execution because a 0. 

It is better, however, is to write and save the script, say with the name mainLinear.m. Then execute it in the Matlab-command window: 

```txt
>> mainLinear
a = -3
x = 0.3333
a = -2
x = 0.5000 
```

```txt
4
a =
-1
x =
1
a =
0
Error using SolveLinear (line 8)
no solution
Error in mainLinear (line 4)
x=SolveLinear(a,b) 
```

we get essentially the same output but it is more convenient to correct errors or change the program. 

## 1.3 The Windows Environment

To run Matlab on a PC, double-click on the Matlab icon. This will present the following screen 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/0d090521d6a60a24e67c71b1b6e194dd7b3c65024210ea468314a03ee09420b7.jpg)


The working directory will depend on where Matlab has been installed. To check in which directory you are, use the command pwd which is the abbreviation for “print working directory”. You then maybe get 

```txt
>> pwd
ans =
C:Users\Administrator\Documents\MATLAB 
```

## 1.3 The Windows Environment

or some similar information. To work in the directory 

```txt
C:Users\myMatlabPrograms 
```

use the command cd which is the abbreviation for “change directory”: 

```txt
>> cd C:Users\myMatlabPrograms
>> pwd
ans =
C:Users\myMatlabPrograms 
```

It is very convenient to work with a script window where you write your programs. Write and store the program under some file name for instance LinearScript.m. Then call it in the Matlab window 

```txt
>> LinearScript 
```

to execute it and get the results. 

To quit Matlab at any time, type quit or exit at the Matlab prompt. If you feel you need more assistance, you can: 

Access the Help Desk by typing doc at the Matlab prompt. 

Type help <subject> at the Matlab prompt, for instance if you like to know more about functions you would type help function. 

Pull down the Help menu on a PC. 

## 1.4 The Linux Environment

In a shell you call matlab and Matlab will present the following screen 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/03f568541a2790c77d38010c04cd0e8cfbd6b7fa20f0c6517dbf4f729d75e3e3.jpg)


If you don’t want to work with the GUI then call matlab -n to obtain Matlab in the same shell without desktop: 

```txt
gander@pnb-502:~$ matlab -n
Starting matlab as: /home/system/opt/matlab/default/bin/matlab
< MATLAB (R) >
Copyright 1984-2013 The MathWorks, Inc.
R2013a (8.1.0.604) 64-bit (glnxa64)
February 15, 2013
To get started, type one of these: helpwin, helpdesk, or demo.
For product information, visit www.mathworks.com.
>> 
```

## 1.5 Using GNU Octave

Matlab without GUI looks very similar to GNU Octave. We start it here and call SolveLinear(3,5): 

```txt
gander@pnb-502:~$ octave
GNU Octave, version 3.2.4
Copyright (C) 2009 John W. Eaton and others.
This is free software; see the source code for copying conditions.
There is ABSOLUTELY NO WARRANTY; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. For details, type 'warranty'.

Octave was configured for "x86_64-pc-linux-gnu".

Additional information about Octave is available at http://www.octave.org.

Please contribute if you find this software useful.
For more information, visit http://www.octave.org/help-wanted.html

Report bugs to <bug@octave.org> (but first, please read http://www.octave.org/bugs.html to learn how to write a helpful report).

For information about changes from previous versions, type 'news'.

octave:1> SolveLinear(3,5)
ans = -1.6667
octave:2> 
```

Newer versions of GNU Octave have also a GUI very similar to Matlab. 

## 1.6 Documenting Results

An easy way to store results generated by computations is to use the command diary. Assume you file LinearScript.m contains the following lines 

## 1.6 Documenting Results

```matlab
% solves the linear equation a*x+b=0 for x.
a=input('a=?')
b=input('b=?')
if a~=0,
    x=-b/a
elseif b==0,
    disp('any x is solution')
else
    disp('no solution')
end 
```

If you use the diary command, you can store the results on a file. Assume you want to store the results on the file MyResuts.txt. The you should write 

```txt
>> diary MyResults.txt
>> LinearScript
a=?3
a =
    3
b=?5
b =
    5
x =
    -1.6667
>> diary off 
```

The file MyResults.txt will be generated in the same directory and contain the session above: 

```txt
LinearScript
a=?3
a =
    3
b=?5
b =
    5
x =
    -1.6667
diary off 
```

## 1.7 MATLAB-Elements Used in This Chapter

The description of the Matlab-elements is taken from the documentation center of the MathWorks Webpage http://www.mathworks.com/. 

format compact: Suppresses excess line feeds to show more output in a single screen. 

M-file: executable Matlab file containing Matlab-commands. It has to be stored in the same directory where Matlab is called. You can use the Matlab-editor or any other text editor to create your .m-files. The files must be stored as plain ASCII text-files with .m-extension. 

pwd: Identify current folder 

cd: Change current folder 

cd (newFolder) changes the current folder to newFolder. 

ls: List folder contents 

ls lists the contents of the current folder. 

quit: Terminate MATLAB program 

exit: Terminate MATLAB program (same as quit) 

doc: Reference page in Help browser doc name displays documentation for the functionality specified by name, such as a function, class, or block. 

help: Help for functions in Command Window help name displays the help text for the functionality specified by name, such as a function, method, class, or toolbox. 

diary: Save Command Window text to file diary(‘filename’) writes a copy of all subsequent keyboard input and the resulting output (except it does not include graphics) to the named file, where filename is the full pathname or filename is in the current MATLAB folder. 

diary off suspends the diary. 

if-statement: See the script LinearScript.m. It has the form 

```ruby
if expression
    statements
elseif expression
    statements
else
    statements
end 
```

%: The percent sign is used to comment out a line. Comments are also useful for program development and testing—comment out any code that does not need to run. To comment out multiple lines of code, you can use the block comment operators, %{ and %}. The %{ and %} operators must appear alone on the lines that comment out the block. Do not include any other text on these lines. 

for: 

Execute statements specified number of times 

for index = values program statements 

end 

values has one of the following forms: 

initval:endval increments the index variable from initval to endval by 1, and repeats execution of program statements until index is greater than endval. 

initval:step:endval increments index by the value step on each iteration, or decrements when step is negative. 

valArray creates a column vector index from subsequent columns of array valArray on each iteration. For example, on the first iteration, index = valArray(:,1). The loop executes for a maximum of n times, where n is the number of columns of valArray,givenbynumel(valArray, 1, :).Theinput valArray can be ofany MATLAB data type, including a string, cell array, or struct. 

input: Used to enter input from the keyboard. 

result = input(prompt) displays the prompt string on the screen, waits for input from the keyboard, evaluates any expressions in the input, and returns the result. 

disp: Used to display things on the screen. disp(X) displays the contents of X without printing the variable name. 

function: See our function SolveLinear. 

function [y1,...,yN] = myfun(x1,...,xM) declares a function named myfun that accepts inputs x1,...,xM and returns outputs y1,...,yN. 

error: Display message and abort function. 

## 1.8 Problems and Exercises

1. Start Matlab with the GUI and watch the introductory video and study the tutorial. 

2. If you own a computer or laptop without Matlab then download and install the open source software GNU Octave on it. 

# Chapter 2 How a Computer Calculates

This section is an excerpt of the material presented in Chap. 2 of [3]. It is important to realize that a computer cannot perform numerical computations exactly like one would expect them to be done in mathematics. Understanding its limitations is essential for developing good programs. 

## 2.1 Finite Arithmetic

A computer is a finite automaton. This means that a computer can only store afinite set ofnumbers and perform only afinite number ofoperations. In mathematics, we are familiar calculating with real numbers R covering the continuous interval $( - \infty , \infty )$ , but on the computer, we must contend with a discrete, finite set of machine numbers $\mathbb { M } = \{ - \tilde { a } _ { m i n } , \dots , \tilde { a } _ { m a x } \}$ . Hence each real number a has to be mapped onto a machine number a to be used on a computer. 

In addition the finite set of machine numbers M contains only real numbers with a limited fix number of digits. If this fixed number of digits is 8 then all numbers with the same leading 8 digits will be mapped to the same machine number. The machine numbers are represented as floating point numbers (here as example in base 10) that is 

$$
\tilde {a} = \pm m \times 1 0 ^ {\pm e}
$$

with $\ l _ { m } = D \ l . D \ l \cdots D$ the mantissa, $e = D \cdots D$ the exponent and D is a digit $\textit { D } \in \{ 0 , 1 , \ldots , 9 \}$ . A nonzero machine number $\tilde { a } \ \ne \ 0$ is (to avoid ambiguity) normalized which means, that the digit before the decimal point in the mantissa is nonzero. The machine numbers are not spread regularly. They are dense near zero and sparse at the end of the computation range $[ - \tilde { a } _ { m i n } , \tilde { a } _ { m a x } ]$ 

If a calculation leads to a result outside the computation range, then we speak of overflow. There exists a smallest positive normalized machine number m. If we compute $b = m / 2$ then we would expect the result to be 0 because there is no normalized machine number between 0 and m. Therefore the interval $( - m , m )$ is called the underflow range (but notice that IEEE arithmetic allow computations with denormalized numbers). 

The machine precision is traditionally defined to be the smallest machine number $e p s > 0$ such that on the computer 

$$
1 + e p s > 1
$$

holds. Newer definition just define eps as the spacing ofthe machine numbers in the interval [1, 2]. 

## 2.2 Rounding Errors

Let $\tilde { a }$ and $\tilde { b }$ be two machine numbers; then $c = \tilde { a } \times \tilde { b }$ will in general not be a machine number anymore, since the product of two numbers contains twice as many digits. The computed result will therefore be rounded to a machine number $\tilde { c }$ which is closest to $c .$ 

As an example, consider the 8-digit decimal machine numbers 

$$
\tilde {a} = 1. 2 3 4 5 6 7 8 \mathrm{and} \tilde {b} = 1. 1 1 1 1 1 1 1,
$$

whose product is 

$$
c = 1. 3 7 1 7 4 1 9 8 6 2 8 2 5 8 \text { and } \tilde {c} = 1. 3 7 1 7 4 2 0.
$$

The absolute rounding error is the difference $r _ { a } = \tilde { c } - c = 1 . 3 7 1 7 4 2 e - 8$ , and 

$$
r = \frac {r _ {a}}{c} = 1 e - 8
$$

is called the relative rounding error. 

On today’s computers, basic arithmetic operations obey the standard model of arithmetic: for $a , b \in \mathbb { M }$ , we have 

$$
a \tilde {\oplus} b = (a \oplus b) (1 + r),\tag{2.1}
$$

where $r$ is the relative rounding error with $| r | < e p s$ , the machine precision. We denote with $\oplus \in \{ + , - , \times , / \}$ the exact basic operation and with $\tilde { \oplus }$ the equivalent computer operation. 

Another interpretation of the standard model of arithmetic is due to Wilkinson. In what follows, we will no longer use the multiplication symbol $\times$ for the exact operation; it is common practice in algebra to denote multiplication without any symbol: ab $\cdot \Longleftrightarrow a \times b$ . Consider the operations 

## 2.2 Rounding Errors

Addition: 

$$
a \tilde {+} b = (a + b) (1 + r) = (a + a r) + (b + b r) = \tilde {a} + \tilde {b}
$$

Subtraction: 

$$
\tilde {a - b} = (a - b) (1 + r) = (a + a r) - (b + b r) = \tilde {a} - \tilde {b}
$$

Multiplication: 

$$
a \tilde {\times} b = a b (1 + r) = a (b + b r) = a \tilde {b}
$$

Division: 

$$
\tilde {a / b} = (a / b) (1 + r) = (a + a r) / b = \tilde {a} / b
$$

In each of the above, the operation satisfies 

## Wilkinson’s Principle

The result of a numerical computation on the computer is the exact result with slightly perturbed initial data. 

For example, the numerical result of the multiplication $\tilde { a \times b }$ is the exact resul $a \tilde { b }$ with a slightly perturbed operand ${ \tilde { b } } = b + b r$ 

## Cancellation

A special rounding error is called cancellation. If we subtract two almost equal numbers, leading digits are canceled. Consider the following two numbers with 5 decimal digits: 

$$
\begin{array}{c} 1. 2 3 4 5 e 0 \\ - 1. 2 3 4 4 e 0 \\ \hline 0. 0 0 0 1 e 0 = 1. 0 0 0 0 e - 4 \end{array}
$$

If the two numbers were exact, the result delivered by the computer would also be exact. But if the first two numbers had been obtained by previous calculations and were affected by rounding errors, then the result would at best be 1.XXXXe 4, where the digits denoted by X are unknown. 

## 2.3 IEEE-Arithmetic

Since 1985 we have for computer hardware theANSI/IEEE Standard 754for Floating Point Numbers. It has been adopted by almost all computer manufacturers. The base is B 2. Expressed as decimal numbers this standard allows to represent numbers with about 16 decimal digits and an exponent of 3-digits. More precisely the computation range is the interval 

$$
\mathbb {M} = \left[ - \tilde {a} _ {\min}, \tilde {a} _ {\max} \right] = \left[ - 1. 7 9 7 6 9 3 1 3 4 8 6 2 3 1 6 e + 3 0 8, 1. 7 9 7 6 9 3 1 3 4 8 6 2 3 1 6 e + 3 0 8 \right]
$$

The standard defines single and double precision floating point numbers. 

Matlab has also adopted IEEE-Arithmetic and computes by default with double precision. We shall not discuss the single precision which uses 32 bits. 

The IEEE double precision floating point standard representation uses a 64-bit word with bits numbered from 0 to 63 from left to right. The first bit S is the sign bit, the next eleven bits E are the exponent bits for e and the final 52 bits F represent the mantissa m: 

$$
\begin{array}{c} \overbrace {E E E E E E E E E E E} ^ {e} \overbrace {F F F F F \cdots F F F F F} ^ {m} \\ 0 1 \quad 1 1 1 2 \quad 6 3 \end{array}
$$

The value a represented by the 64-bit word is defined as follows: 

normal numbers: 

If 0 < e < 2047, then $\tilde { a } = ( - 1 ) ^ { S } \times 2 ^ { e - 1 0 2 3 } \times 1$ .m where 1.m is the binary number created by prefixing m with an implicit leading 1 and a binary point. 

subnormal numbers: 

If e 0 and m 0, then $\tilde { a } = ( - 1 ) ^ { S } \times 2 ^ { - 1 0 2 2 } \times 0 . m$ which are denormalized numbers. 

If e 0 and m 0 and S 1, then a 0 

exceptions: 

If e 2047 and m 0, then a NaN (Not a number) 

If e 2047 and m 0 and S 1, then a Inf 

Using the hexadecimalformat in Matlab we can see the internal representation of a floating point number. We obtain for example 

```txt
>> format hex
>> 2
ans = 400000000000000 
```

If we expand each hexadecimal digit to 4 binary digits we obtain the bit pattern for the floating point number 2: 

```txt
0100 0000 0000 0000 0000 0000 .... 0000 0000 0000 
```

We skipped with .... seven groups of four zero binary digits. The interpretation is: 1 21024−1023 1.0 2. 

```txt
>> 6.5
ans = 401a000000000000 
```

This means 

```txt
0100 0000 0001 1010 0000 0000 .... 0000 0000 0000 
```

Again we skipped with .... seven groups of four zeros. The resulting number is $\begin{array} { r } { + 1 \times 2 ^ { 1 0 2 5 - 1 0 2 3 } \times ( 1 + \frac { 1 } { 2 } + \frac { 1 } { 8 } ) = 6 . 5 . } \end{array}$ 

From now on, we will stick to the IEEE Standard as used in Matlab. In other, more low-level programming languages, the behavior of the IEEE arithmetic can be adapted, e.g. the exception handling can be explicitly specified. 

The machine precision is $e p s = 2 ^ { - 5 2 }$ 

The largest machine number $\tilde { a } _ { m a x }$ is denoted by the constant realmax. Note that 

```txt
>> realmax
ans = 1.7977e+308 
```

The computation range is the interval realmax, realmax . If an operation produces a result outside this interval, then it is said to overflow. Before the IEEE Standard, computation would halt with an error message in such a case. Now the result of an overflow operation is assigned the number Inf. 

The smallest positive normalized number is realmin 2−1022. 

IEEE allows computations with denormalized numbers. The positive denormalized numbers are in the interval realmin eps, realmin . If an operation produces a strictly positive number that is smaller than realmin eps, then this result is said to be in the underflow range. Since such a result cannot be represented, zero is assigned instead. 

When computing with denormalized numbers, we may suffer a loss of precision. Consider the following Matlab program: 

```txt
>> format long
>> res=pi*realmin/123456789101112
res = 5.681754927174335e-322
>> res2=res*123456789101112/realmin
res2 = 3.15248510554597
>> pi = 3.14159265358979 
```

The first result res is a denormalized number, and thus can no longer be represented with full accuracy. So when we reverse the operations and compute res2, we obtain a result which only contains 2 correct decimal digits. We therefore recommend avoiding the use of denormalized numbers whenever possible. 

## 2.4 MATLAB-Elements Used in This Chapter

eps: the machine precision eps returns the distance from 1.0 to the next largest double-precision number, that is eps 2−52. 

realmin: Smallest positive normalized floating-point number. n realmin returns the smallest positive normalized floating-point number in IEEE double precision. 

realmax: Largest positive floating-point number. n realmax returns the largest finite floating-point number in IEEE double precision. 

format: format sets the display of floating-point numeric values to the default display format, which is the short fixed decimal format. This format displays 5-digit scaled, fixed-point values. 

format hex: Hexadecimal representation of a binary double-precision number. 

NaN: Not-a-Number 

NaN returns the IEEE arithmetic representation for Not-a-Number (NaN). These values result from operations which have undefined numerical results. 

Inf: Infinity 

Inf returns the IEEE arithmetic representation for positive infinity. Infinity values result from operations like division by zero and overflow, which lead to results too large to represent as conventional floating-point values. 

## 2.5 Problems

1. Consider the following finite decimal arithmetic: 2 digits for the mantissa and one digit for the exponent. So the machine numbers have the form $\pm Z . Z \mathrm { E } \pm Z$ where $Z \in \{ 0 , 1 , \ldots , 9 \}$ 

(a) How many normalized machine numbers are available? 

(b) Which is the overflow- and the underflow range? 

(c) What is the machine precision? 

(d) What is the smallest and the largest distance of two consecutive machine numbers? 

2. Solving a quadratic equation: Write a Matlab function 

function [x1,x2]=QuadraticEq(p,q) 

which computes the real solutions of an equation 

$$
x ^ {2} + p x + q = 0.
$$

If the solutions turn out to be complex then write an error message. Test your program with the following examples: 

$( x - 2 ) ( x + 3 ) = x ^ { 2 } + x - 6 = 0 \quad { \mathrm { t h u s ~ } } p = 1 { \mathrm { ~ a n d ~ } } q = - 6 .$ 

$$
(x - 1 0 ^ {9}) (x + 2 \cdot 1 0 ^ {- 9}) = x ^ {2} + (2 \cdot 1 0 ^ {- 9} - 1 0 ^ {9}) x + 2
$$

thus $p = 2 e { - } 9 - 1 e 9 \mathrm { a n d } q = - 1 e 9 .$ 

(x 10<sup>200</sup>)(x 1) x<sup>2</sup> (10<sup>200</sup> 1)x 10<sup>200</sup> 

thus $p = 1 e 2 0 0 - 1$ and $q = - 1 e 2 0 0$ 

Comment your results. 

# Chapter 3 Plotting Functions and Curves

In this section we learn how to define functions in Matlab and how functions and curves can be plotted. 

## 3.1 Plotting a Function

Assume we would like to plot the function f(x) 1 sin x for $x \in [ 0 , 2 \pi ]$ . First we have to program the function. One way to do this is to write a file with the name f.m and store it in the same directory where Matlab was called. The file f.m looks as follow 

```javascript
function y=f(x)
y=1+sin(x); 
```

In the Matlab-window we can evaluate this function 

```txt
>> y=f(0)
y =
1
>> y=f(pi/4)
y =
1.7071 
```

Notice that pi is a predefined constant in Matlab. 

```txt
>> pi
ans =
3.1416 
```

also the imaginary unit i or 1i is predefined: 

```python
>> i
ans =
    0.0000 + 1.0000i
>> 1i
ans =
    0.0000 + 1.0000i
>> 1i^2
ans =
    -1 
```

It is better to use 1i in order to have the variable i free for other purposes. 

Since machine number are a finite set we cannot really plot a continuous function. We can only sample the function for say n equidistant values of x and connect adjacent values by a straight line. Assume we compute n 7 values of our function. In Matlab we store the values in a vector (that is a one dimensional array). We define the spacing between two function values by h: 

```txt
>> h=2*pi/7
h =
0.8976
>> x=0:h:2*pi
x =
Columns 1 through 7
0 0.8976 1.7952 2.6928 3.5904 4.4880 5.3856
Column 8
6.2832 
```

Notice the construction of this vector x. It has the form 

```txt
x=startvalue : stepsize : endvalue 
```

For each value of the vector x we want to evaluate our function. This can be done in Matlab very compactly by just calling f with the vector x as argument 

```txt
>> y=f(x)
y =
Columns 1 through 7
1.0000 1.7818 1.9749 1.4339 0.5661 0.0251 0.2182
Column 8
1.0000 
```

Now we have computed two vectors x and y and we can connect the function values by the plot command by straight line segments: 

```lisp
plot(x,y) 
```

we get a new graphic window with the function plot (see first plot in Fig. 3.1). It does not look very good. The spacing between the function values is too large! We can easily improve this by using more function values: 

```lisp
x=0:0.01:2*pi;
plot(x, f(x)) 
```

## 3.1 Plotting a Function

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/3e34d44eed6726b637f2f1a63870921e0f0778f12bae3c6cf1762dadadd140a9.jpg)



Fig. 3.1 Plotting a function with different spacing


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/b33716d158211631b45cbe18a7556a1f1ec4f08c6dd3c67e47871c73b992467b.jpg)


Now the plot looks much better (see second plot in Fig. 3.1). 

Note that there is a Matlab-function called linspace: 

```txt
>> x=1inspace(0,2*pi) 
```

it returns in x 100 equidistant values in the interval 0, 2 . If you need 500 values you can write x=linspace(0,2<sub>*</sub>pi,500). 

Standard functions in Matlab can be called with vectors as arguments as we just saw for $f ( x ) = 1 + \sin ( x )$ . For a vector ${ \pmb x } = ( x _ { 1 } , \dots , x _ { n } )$ the function sin(x) computes 

$$
\sin (\boldsymbol {x}) = [ \sin x _ {1}, \sin x _ {2}, \dots , \sin x _ {n} ].
$$

By adding 1 sin(x) the term 1 is expanded to 

```julia
ones (size(x)) + sin(x) 
```

so that the result is 

$$
1 + \sin (\boldsymbol {x}) = [ 1 + \sin x _ {1}, 1 + \sin x _ {2}, \dots , 1 + \sin x _ {n} ].
$$

When we wish to construct functions that allow vectors as arguments we need to use the dot operations. These are element by element operations. Consider for instance the function. 

$$
g (x) = \frac {\sin (x)}{e ^ {x}}.
$$

Programming this function as 

```javascript
function y=g(x)
y=sin(x)/exp(x); 
```

would not allow to call g(x) with a vector as argument. However, if we program g as 

```javascript
function y=g(x)
y=sin(x)./exp(x); 
```

then the elements of the two vectors are divided element-wise and the result is what we want. 

## 3.2 Plotting Curves

If we wish to plot a circle with center $C = ( c _ { 1 } , c _ { 2 } )$ and radius r we need to know the equation of the circle. In Cartesian coordinates the equations reads 

$$
(x - c _ {1}) ^ {2} + (y - c _ {2}) ^ {2} = r ^ {2}.
$$

Now to plot the circle in this representation we would have to solve the equation for y and we would obtain two functions $y ( x )$ . Then we need to compute say 30 x-values in the interval $( c _ { 1 } - r , c _ { 1 } + r )$ and plot the two half-arcs for the two values of y. 

There is a much simpler solution. We represent the same circle using a parameter t by 

$x(t) = r\cos t$ $y(t) = r\sin t,\quad t = 0,\ldots ,2\pi .$ 

Then we write 

```txt
clear, clf
r=2
C=[0.5,1]
t=linspace(0,2*pi,60)
axis([-3,4,-2,4])
axis equal
hold
plot(C(1)+r*cos(t), C(2)+r*sin(t))
plot(C(1),C(2),'x') 
```

to get the plot in Fig. 3.2. 

## 3.3 Plotting 3-d Curves

Consider to plot the space curve 

$x(t) = 3\cos t$ $y(t) = 5\sin t$ $z(t) = 2t.$ 

```txt
>> t = 0:pi/50:10*pi;
>> plot3(3*cos(t), 5*sin(t), 2*t)
we obtain Fig.3.3. 
```

## 3.3 Plotting 3-d Curves


Fig. 3.2 Plotting a circle using parametric representation


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/60be0203c308192fa4bae132ac014a79ebb93d1bc7aadb278ce1f183b476122f.jpg)



Fig. 3.3 Plotting a space curve


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/4ed66aeb5bad73bfcff54214c3ad6dec2d57a03604da73126dd507884aff7f83.jpg)


Using the function plot3 and 

## 3.4 Surface and Mesh Plots

Matlab offers many functions for visualizing. See the description on http://www. mathworks.com/help/matlab/surface-and-mesh-plots-1.html. To visualize the surface of a two dimensional function one has to define first a grid in the xy-plane on which the function will be evaluated. The grid is defined with the function meshgrid. For instance with 

```matlab
>> [x,y] = meshgrid(-1:1:1,0:1:3)
x =
-1 0 1
-1 0 1
-1 0 1
-1 0 1 
```

<table><tr><td>Y =</td><td></td><td></td><td></td></tr><tr><td></td><td>0</td><td>0</td><td>0</td></tr><tr><td></td><td>1</td><td>1</td><td>1</td></tr><tr><td></td><td>2</td><td>2</td><td>2</td></tr><tr><td></td><td>3</td><td>3</td><td>3</td></tr></table>

we get a grid of 12 points with the coordinates 

<table><tr><td>(-1,0)</td><td>(0,0)</td><td>(1,0)</td></tr><tr><td>(-1,1)</td><td>(0,1)</td><td>(1,1)</td></tr><tr><td>(-1,2)</td><td>(0,2)</td><td>(1,2)</td></tr><tr><td>(-1,3)</td><td>(0,3)</td><td>(1,3)</td></tr></table>

To evaluate the function $f ( x , y ) = x ^ { 2 } + y ^ { 2 }$ on that grid we compute 

>> F=x. $^{2}$ +y. $^{2}$ F =
1 0 1
2 1 2
5 4 5
10 9 10 

To plot the surface of the function, Matlab offers two possibilities. The first one connects the function values in both directions by a mesh: 

```txt
>> mesh(x,y,F) 
```

see the left picture in Fig. 3.4. The second possibility is to connect the Function values by surfaces: 

```txt
>> surf(x,y,F) 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/39cf8675f7c44ca75acf11982d5c422e443fd32887b86b306e5adac452a8f76f.jpg)



Fig. 3.4 mesh and surf function


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/7a0b5bb37ad56c53268f4a0f350745362c0a00f69b197780fc5c07a16debbf43.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/6e60c5ebb05647be08b9c62d3b6657f59586cd931a47da741594eb4f92c871cd.jpg)



Fig. 3.5 Finer grid for mesh and surf


We obtain the right plot in Fig. 3.4. Both figures look nicer if we use a finer grid: 

```txt
[x,y] = meshgrid(-1:0.1:1,0:0.1:3)
F=x.^2+y.^2
mesh(x,y,F)
surf(x,y,F) 
```

We get the plots in Fig. 3.5. 

## 3.5 Contour Plots

A two dimensional function can also be represented by level lines as a contour plot. Consider the function 

$$
f (x, y) = \cos (y \cos (x)).
$$

To see the level lines of the function in the domain $- \pi \leq x \leq \pi$ and $0 \leq y \leq 2 \pi$ we program 

```matlab
x=linspace(-pi, pi);
y=linspace(0, 2*pi);
[X, Y]=meshgrid(x, y);
Z=cos(Y.*cos(X));
figure(1)
contour(X, Y, Z)
figure(2)
mesh(Z) 
```

We obtain Fig. 3.6. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/1558e0fe95a88c2bc3d35703a7e6085a78ad78c3af10fcdc598287654f834f37.jpg)



Fig. 3.6 Contour and mesh plot


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/bb996d0587013e02482c709c6fff2b93de9ad2a117cd2b74ea4d7bc60ade0536.jpg)


## 3.6 MATLAB-Elements Used in This Chapter

pi: Predefined constant π 3.141592653589793. 

1i, i: the imaginary unit. It is recommended to use 1i since i may be overwritten and used as variable. 

clf: Clear current figure window. 

clear: clear removes all variables from the current workspace, releasing them from system memory. 

axis: Axis scaling and appearance. axis([xmin xmax ymin ymax]) sets the limits for the x- and y-axis of the current axes. axis equal sets the aspect ratio so that the data units are the same in every direction. This is important to let a circle not appear as an ellipse! 

plot: We have used here the simplest form 1 plot(X,Y) creates a 2-D line plot of the data in Y versus the corresponding values in X. There are many useful other Matlab-function available, see http://www.mathworks.com/help/matlab/line-plots.html. A whole gallery of plot possibilities is discussed on http://www. mathworks.com/discovery/gallery.html?s_tid=abdoc_plot. 

colon (:) : Create vectors, array subscripting, and for-loop iterators 

linspace: This function generates linearly spaced vectors. 

$\mathrm { { y } = \ l i n s p a c e { ( a , b ) } }$ generates a row vector y of 100 points linearly spaced between and including a and b. y linspace(a,b,n) generates a row vector y of n points linearly spaced between and including a and b. 

ones: Create array ofall ones. Example $\mathtt { A = o n e s } \left( 3 , 2 \right)$ creates a $3 \times 2$ matrix with all elements 1. 

size: Array dimensions 

$\mathrm { d } = \mathrm { s i z e } ( \mathrm { X } )$ returns the sizes of each dimension of array X in a vector, d, with ndims(X) elements. 

length: Length of vector or largest array dimension 

numberOfElements length(array) finds the number ofelements along the largest dimension of an array. array is an array of any MATLAB data type and any valid dimensions. numberOfElements is a whole number of the MATLAB double class. For nonempty arrays, numberOfElements is equivalent to max(size(array)). For empty arrays, numberOfElements is zero. 

clf: Clear current figure window 

clf deletes from the current figure all graphics objects whose handles are not hidden (i.e., their HandleVisibility property is set to on). 

: The -operator is used to solve a system of linear equations. If you are given the matrix A and the right hand side b of a system of linear equations 

$$
A \boldsymbol {x} = \boldsymbol {b}
$$

then the solution is computed in Matlab with 

$$
> > x = A \backslash b
$$

## dot-operations:

a dot preceding the operators $\star \ , \quad / \ , \quad \ \stackrel { \sim } { }$ causes an element-byelement operation. Thus if x and y are vectors of the same length then 

$$
\mathrm{x.} * \mathrm{y} = [ x _ {1} y _ {1}, x _ {2} y _ {2}, \dots , x _ {n} y _ {n} ].
$$

plot3: The plot3 function displays a three-dimensional plot of a set of data points. 

meshgrid: Rectangular grid in 2-D space. 

[X,Y] = meshgrid(xgv,ygv) replicates the grid vectors xgv and ygv to produce a full grid. This grid is represented by the output coordinate arrays X and Y. The output coordinate arrays X and Y contain copies of the grid vectors xgv and ygv respectively. The sizes of the output arrays are determined by the length of the grid vectors. For grid vectors xgv and ygv of length M and N respectively, X and Y will have N rows and M columns. 

mesh: Mesh plot. 

mesh(X,Y,Z) draws a wireframe mesh with color determined by Z, so color is proportional to surface height. IfX and Y are vectors, length(X) n and length(Y) m, where $[ \mathrm { m , n } ] = \mathrm { s i z e } ( Z )$ In this case, (X(j), Y(i), Z(i,j)) are the intersections of the wireframe grid lines; X and Y correspond to the columns and rows of Z, respectively. If X and Y are matrices, $( \mathrm { X } ( \mathrm { i , j } ) , \mathrm { Y } ( \mathrm { i , j } ) , \mathrm { Z } ( \mathrm { i , j } ) )$ are the intersections of the wireframe grid lines. 

## surf: 3-D shaded surface plot.

surf(X,Y,Z) uses Z for the color data and surface height. X and Y are vectors or matrices defining the x and y components of a surface. If X and Y are vectors, length(X) n and length(Y) m, where $[ \mathrm { m , n } ] = \mathrm { s i z e } ( Z )$ . In this case, the vertices of the surface faces are (X(j), Y(i), Z(i,j)) triples. To create X and Y matrices for arbitrary domains, use the meshgrid function. 

## contour: draws a contour plot of a matrix.

contour(Z) draws a contour plot of matrix Z, where Z is interpreted as heights with respect to the x-y plane. Z must be at least a 2-by-2 matrix that contains at least two different values. The x values correspond to the column indices of Z and the y values correspond to the row indices of Z. The contour levels are chosen automatically. 

contour(Z,n) draws a contour plot of matrix Z with n contour levels where n is a scalar. The contour levels are chosen automatically. 

## hold: Retain current graph when adding new graph

The hold function controls whether MATLAB clears the current graph when you make subsequent calls to plotting functions (the default), or adds a new graph to the current graph. 

## 3.7 Problems

## 1. We are given the points

<table><tr><td>x</td><td>0.9</td><td>2.3</td><td>3.9</td><td>4.6</td><td>5.8</td><td>7.3</td></tr><tr><td>y</td><td>2.9</td><td>4.1</td><td>4.8</td><td>7.0</td><td>7.0</td><td>8.7</td></tr></table>

(a) Define a region to plot the points using axis. Use hold to freeze the axis. 

(b) Plot the points using the symbol $\cdot _ { \mathrm { x } } ,$ 

(c) We want to fit a regression line through the points, that means compute the parameters a and b such that 

$$
y _ {k} = a x _ {k} + b, \quad k = 1, \dots , 6.
$$

This is a linear system of equations with two unknowns and 6 equations. It cannot be solved exactly, the equations contradict themselves. However, the Matlab -operator does solve the system in the least squares sense by computing the best approximation for all equations. 

Form the linear system $A \left( ^ a _ { b } \right) = { \bf y }$ and solve it by $\mathtt { A } \backslash \mathtt { y }$ 

(d) Using the computed values of a and b, plot the regression line on the same plot with the points. 

## 2. Ellipse plots.

(a) Plot the ellipse with center in origin and the main axis $a = 3$ on the x-axis and minor axis $b = 1$ . Plot also the center using the symbol $\cdot _ { + } ,$ 

(b) Now move the ellipse so that the center is the point $( 4 , - 1 )$ and the direction of the main axis has an angle of $- 3 0 ^ { \circ }$ with the x-axis. Plot this new ellipse in the same frame. 

Hint: Use a rotation matrix of the form 

$$
Q = \left( \begin{array}{c c} \cos \alpha & - \sin \alpha \\ \sin \alpha & \cos \alpha \end{array} \right)
$$

to rotate the coordinates of the ellipse. 

3. Plot for $- 3 \leq x \leq 3$ and $- 5 \leq y \leq 5$ the function $f ( x , y ) = x ^ { 2 } - 2 y x ^ { 3 }$ using contour and mesh. 

## Chapter 4 Some Elementary Functions

Standard functions are available in almost all programming languages. But how could we actually compute them by using only the 4 basic arithmetic operations $\{ + , - , \times , / \} \ i$ Algorithms for computing standard functions on computers were developed some 60 years ago. Today many of them are part of the hardware. In spite of that it is interesting and challenging to try to develop a good algorithm for some well known functions. 

A useful tool to evaluate a function is its Taylor expansion: 

$$
f (x) = f (a) + \frac {f ^ {\prime} (a)}{1 !} h + \dots + \frac {f ^ {(n)} (a)}{n !} h ^ {n} + R _ {n} (a, x),\tag{4.1}
$$

with $h = x - a$ . For the remainder we have the estimate 

$$
\left| R _ {n} (x, a) \right| \leq \frac {\left| f ^ {(n + 1)} (\xi) \right|}{(n + 1) !} | h | ^ {n + 1}
$$

where $\xi$ is a number between a and x. If the function is infinitely differentiable then the remainder converges for $n \to \infty$ and for some r ( the radius of convergence) for all $| x - a | < r$ to zero. Thus we get the Taylor series 

$$
f (x) = \sum_ {i = 0} ^ {\infty} \frac {f ^ {(i)} (a)}{i !} (x - a) ^ {i},\tag{4.2}
$$

which represents the function for $| x - a | < r$ . If the expansion point $a = 0$ then the series is called Maclaurin-series. 

## 4.1 Computing the Exponential Function

For $f ( x ) = e ^ { x }$ all derivatives exist $f ^ { ( n ) } ( x ) = e ^ { x }$ thus with $f ^ { ( n ) } ( 0 ) = 1$ the Maclaurinseries becomes 

$$
e ^ {x} = \sum_ {i = 0} ^ {\infty} \frac {x ^ {i}}{i !}.\tag{4.3}
$$

One can show that in this case the radius of convergence is $r = \infty$ , thus Eq. (4.3) can be used to compute $e ^ { x }$ for any x. Let’s develop a program to sum up the series (4.3). The term 

$$
a _ {i} = \frac {x ^ {i}}{i !}
$$

can be computed by updating the preceding term $a _ { i - 1 }$ through 

$$
a _ {i} = \frac {x}{i} a _ {i - 1}.
$$

We denote by sn the new and by so the old partial sum. We terminate the summation when the relative difference between the new and the old partial sum is smaller than $1 0 ^ { - 6 }$ . Thus we obtain a first version: 

```matlab
function sn=e1(x);
%
so=0; sn=1; term=1; k=1;
while abs(sn-so)>1e-6*sn
    so=sn; term=term*x/k;
    sn=so+term; k=k+1;
end

Indeed we obtain

>> for x=[1,-1,10,-10,20,-20]
    [e1(x) exp(x)]
    end

ans =
    2.718281801146385    2.718281828459046
ans =
    0.367879464285714    0.367879441171442
ans =
    1.0e+04 *
    2.202646026627129    2.202646579480672
ans =
    1.0e-04 *
    0.453999364851671    0.453999297624848
ans =
    1.0e+08 *
    4.851649751360876    4.851651954097902
ans =
    1.0e-08 *
    0.562188480727156    0.206115362243856 
```

quite good results except for $x = - 2 0$ . We shall explain in the exercises why this algorithm fails for large negative arguments. Since the algorithm seems to work well for $x > 0$ we can make it work also for negative arguments by using the relation 

$$
e ^ {- x} = \frac {1}{e ^ {x}}\tag{4.4}
$$

thus compute first $s = e ^ { | x | }$ and then adjust the result 

```matlab
if x<0, s=1/s; end 
```

We can also improve the termination criterion. For fixed x the terms 

$$
a _ {k} = \frac {x ^ {k}}{k !} \rightarrow 0, k \rightarrow \infty
$$

converge rapidly to zero. So we shall sum the series until in finite arithmetic we get for the partial sum $s _ { k }$ 

$$
s _ {k} + a _ {k + 1} = s _ {k}.
$$

Thus we get the algorithm 

```matlab
function sn=Exp(x);
% EXP stable computation of the exponential function
% s=Exp(x); computes an approximation s of exp(x) up to machine
% precision. 
```

```matlab
if x<0, v=-1; x=abs(x); else v=1; end
so=0; sn=1; term=1; k=1;
while sn~=so
    so=sn; term=term*x/k;
    sn=so+term; k=k+1;
end
if v<0, sn=1/sn; end; 
```

This program works now perfectly 

```txt
>> for x=[1,-1,10,-10,20,-20]
    (exp(x) - Exp(x)) / exp(x)
    end
ans =
    0
ans =
    1.5089e-16
ans =
    3.3033e-16
ans =
    -2.9851e-16
ans =
    1.2285e-16
ans =
    -2.0066e-16 
```

We obtain results that match the exponential function to machine precision. 

## 4.2 Computing sin and cos

The Taylor series for the two trigonometric functions are obtained by the beautiful relation 

$$
e ^ {i x} = \cos x + i \sin x \quad \text { Euler's   formula }\tag{4.5}
$$

by expanding the Maclaurin series for $e ^ { i x }$ and separating real and imaginary parts: 

$$
\cos x = \sum_ {k = 0} ^ {\infty} \frac {(- 1) ^ {k}}{(2 k) !} x ^ {2 k} = 1 - \frac {x ^ {2}}{2 !} + \frac {x ^ {4}}{4 !} - \dots\tag{4.6}
$$

$$
\sin x = \sum_ {k = 0} ^ {\infty} \frac {(- 1) ^ {k}}{(2 k + 1) !} x ^ {2 k + 1} = x - \frac {x ^ {3}}{3 !} + \frac {x ^ {5}}{5 !} - \dots\tag{4.7}
$$

If we wish to use these expansions for computing cos x or sin x we have to expect numerical problems for large arguments $| x | \gg 1$ . This because the series are alternating and affected by cancellation. The remedy is to reduce first the argument to the interval $[ - \pi / 2 , \pi / 2 ]$ . Then the series can be summed without too much cancellation (see Problem 2). 

## 4.3 Computing arctan

We know that the derivative of $f ( x ) = \arctan x$ is given by 

$$
\frac {d}{d x} \arctan x = \frac {1}{1 + x ^ {2}} = \sum_ {k = 0} ^ {\infty} (- 1) ^ {k} x ^ {2 k}
$$

The series converges for $| x | < 1$ . Thus by integrating we obtain 

$$
\arctan x = \sum_ {k = 0} ^ {\infty} (- 1) ^ {k} \frac {x ^ {2 k + 1}}{2 k + 1} = x - \frac {x ^ {3}}{3} + \frac {x ^ {5}}{5} - \dots\tag{4.8}
$$

We shall use this series to compute arctan in Problem 5. 

## 4.4 MATLAB-Elements Used in This Chapter

for: Execute statements specified number of times. for index=values, program statements, end repeatedly executes one or more Matlab statements in a loop. values can be: 

initval:endval 

increments the index variable from initval to endval by 1, and repeats execution of program statements until index is greater than endval. 

initval:step:endval 

increments index by the value step on each iteration, or decrements when step is negative. 

valArray 

The loop executes for a maximum of n times, where n is the number of columns of valArray. 

while: Repeatedly execute statements while condition is true. 

while expression, statements, end 

repeatedly executes one or more Matlab program statements in a loop as long as an expression remains true 

mod: Modulus after division 

M = mod(X,Y) returns the modulus after division of X by Y. In general, if Y does not equal 0, M = mod(X,Y) returns X - n.*Y, where n = floor(X./Y). If Y is not an integer and the quotient X./Y is within roundoff error of an integer, then n is that integer. Inputs X and Y must have the same dimensions unless one is a scalar double. If one input has an integer data type, then the other input must be of the same integer data type or be a scalar double. (will be used in the problem section) 

## 4.5 Problems

1. Explain what happens in Algorithm e1 when x 20. Hint: look at the size of the largest term and at the final result. What happens when computing the result in finite arithmetic? 

2. Write a Matlab-function to compute sin x using the series (4.7). In order to avoid cancellation for large x reduce the argument to the interva $[ - \pi / 2 , \pi / 2 ]$ 

3. Do the same for cos x. 

4. Combine both functions and write a function to compute tan x. 

5. Write a function to compute arctan x for $| x | < 1$ using the series (4.8) and compare your result with the standard Matlab-function atan(x). 

# Chapter 5 Computing with Multiple Precision

In this section we shall show how to perform some computations with more digits than given by the IEEE floating point arithmetic. The problems of this section will need integer operations and variables of integer data types. It is an opportunity to learn the corresponding Matlab features. 

## 5.1 Computation of the Euler Number e

We shall compute the Euler number $e = \exp ( 1 )$ to an arbitrary number of decimal digits. For this we will use the algorithm e1 in Chap. 4 which we developed to compute the exponential function using the Taylor series. The series is evaluated for for $x = 1$ 

$$
e = \sum_ {k = 0} ^ {\infty} \frac {1}{k !}.\tag{5.1}
$$

Using the notations $a = 1 / k !$ for the kth term and s for a partial sum we get the function 

```matlab
function s=Eulerconstant;
s=1;sn=2; a=1; k=1; % initialization
while s~=sn
    s=sn; k=k+1;
    a=a/k; % new term
    sn=s+a; % new partial sum
end 
```

Indeed we obtain with 

```txt
>> format long
>> s=Eulerconstant
s =
2.718281828459046 
```

a result with 16 decimal digits which is what we can expect by using IEEE-arithmetic. If we want to compute more digits we need to simulate multiple precision arithmetic. In the above algorithm the only arithmetic operations are 

$$
k = k + 1, \quad a = a / k \text { and } s n = s + a.
$$

For k we may use a simple variable. We shall not compute so many terms of the Taylor series that also k has to be represented in multiple precision arithmetic. The partial sum and the terms to be added, however, have to be multiple precision numbers. We shall store the digits of a multiple precision number in a integer array. There are several integer data types in Matlab available. Here we shall use uint32<sup>1</sup>. which is a data type for unsigned integers. 

This function is used for conversion to 32-bit unsigned integers. These 32-bit numbers cover the range from 0 to 2<sup>32</sup> 1 4294967295. Let a be an array of such unsigned integer numbers. We represent the number 1 using 20 digits: 

```txt
>> a=uint32(zeros(1,20));
>> a(1)=1
a =
Columns 1 through 10
    1    0    0    0    0    0    0    0    0
Columns 11 through 20
    0    0    0    0    0    0    0    0    0 
```

If we wish to divide this number by k=2 we should get the result 

```txt
a =
Columns 1 through 10
0    5    0    0    0    0    0    0    0
Columns 11 through 20
0    0    0    0    0    0    0    0    0 
```

Another division by k=3 should give 

```txt
a =
Columns 1 through 10
0 1 6 6 6 6 6 6 6 6
Columns 11 through 20
6 6 6 6 6 6 6 6 6 6 
```

## 5.1 Computation of the Euler Number e

We would like to see the digits not as elements of a vector but continuously as large number. This can be done by using the function sprintf (sprintf formats data into a string of characters). 

```csv
>> sprintf('%01d',a)
ans =
01666666666666666666 
```

Let us program this division. We need to use a function for integer division. In Matlab this is the function idivide. For the remainder we use the function mod. Suppose we want to divide 14 by 3. The result is: quotient = 14/3 = 4 and remainder = mod(14,3) = 2. Programmed in Matlab this is 

```javascript
quotient=idivide(14,3) remainder=mod(14,3) 
```

Thus our division function becomes 

```matlab
function a=Dividel(k,a)
% divides the integer array a by integer number k
n=length(a);
c=10;
remainder=a(1);
for i=1:n-1
    a(i)=idivide(remainder,k);
    remainder=mod(remainder,k)*c+a(i+1);
end
a(n)=idivide(remainder,k); 
```

Let us test this function. The following script divides the initial number a=1 with the numbers k 2, . . . , 15. Thus the last result should be 1/15 : 

```matlab
clear, clc, format long
res=[];
a=zeros(1,30,'uint32');
a(1)=1;
for k=2:15
    a=Divide1(k,a);
    res =[res;sprintf('%01d',a)];
end
res
1/factorial(15) 
```

```txt
res =
0500000000000000000000000000
016666666666666666666666666
00416666666666666666666666
0008333333333333333333333333
000138888888888888888888888
000019841269841269841269841269
000002480158730158730158730158 
```

```txt
000000275573192239858906525573
000000027557319223985890652557
000000002505210838544171877505
000000000208767569878680989792
000000000016059043836821614599
000000000001147074559772972471
000000000000076471637318198164
>> 1/factorial(15)
ans =
    7.647163731819816e-13 
```

It looks good! Notice that the smaller the numbers get the more leading zeros appear. It is not necessary to divide these leading zeros by k since they remain zero. We use the variable imin to count the number of leading zeros in the vector and start the division at position a(imin+1). The division function changes so to 

```matlab
function [A, imin]=Divide(c, imin, k, A)
% DIVISION divides the multiple precision number A by the integer
% number k. The first imin components of A are zero. imin is updated
% after the division. c defines the number of decimal digits in one
% array element: c=10 is used for one digit, c=100 for two digits etc.
n=length(A);
if imin <n    % if imin=n => A=0
    first=1;
    remainder=A(imin+1);
    for i=imin+1:n
    A(i)=idivide(remainder, k);
    if A(i)==0
    if first    % update imin
    imin=i;
    end
    else
    first=0;
    end
    if i<n
    remainder=mod(remainder, k)*c+A(i+1);
    end
    end
end 
```

Notice at the beginning ofthe division the variable imin is updated if a(i) becomes zero. After the first nonzero element the update is stopped. The following test shows that imin counts the leading zeros correctly: 

```matlab
% Testprogram for Divide for c=10 or c=100
clear, clc, format long
a=zeros(1,30,'uint32');
imin=0;
a(1)=1;
c=100;
if c==10, w='%01d'; else w='%02d'; end 
```

## 5.1 Computation of the Euler Number e

```matlab
res = [sprintf('%5d', imin), ' ', sprintf(w, a)];
for k=2:15
    [a, imin]=Divide(c, imin, k, a);
    res = [res; sprintf('%5d', imin), ' ', sprintf(w, a)];
end
res 
```

```c
res = 0 100000000000000000000000000
1 050000000000000000000000000
1 01666666666666666666666666
2 004166666666666666666666666
3 0008333333333333333333333333
3 00013888888888888888888888888
4 000019841269841269841269841269
5 000002480158730158730158730158
6 000000275573192239858906525573
7 000000027557319223985890652557
8 000000002505210838544171877505
9 000000000208767569878680989792
10 00000000016059043836821614599
11 00000000001147074559772972471
13 00000000000076471637318198164 
```

So far we can generate the terms of the series of Eq. (5.1). Next we need to sum up the terms. Let s denote the partial sum and t the next term. The function Add.m is straightforward 

```matlab
function r=Add(imin,s,a);
% ADD adds the multiprecision number a to s without carry. It is
% supposed that s>a and that imin leading components of a are zero
n=length(s);
r=s;
for i=imin+1:n
    r(i)=s(i)+a(i);
end 
```

but we have to take care of possible carry and so we need also to sweep over the array with 

```matlab
function s=Carry(c,s);
% CARRY normalizes the component of s such that 0 <= s(i) < c
% and moves the carry to the next component
n=length(s);
for i=n:-1:2
    while s(i)>=c
    s(i)=s(i)-c; s(i-1)=s(i-1)+1;
    end
end 
```

## Our main program becomes

```matlab
function s=EmultPrec(c,n);
% EMULTPREC computes n*log10(c) decimal digits of
% the Euler constant e=exp(1). The digits are stored
% in the array s.
a=zeros(1,n,'uint32');    % define array of
s=a;    % unsigned integers
a(1)=1; s(1)=2;
k=1; imin=0;    % imin skips leading zeros
while imin<n
    k=k+1;
    [a,imin]=Divide(c,imin,k,a);    % new term
    s=Add(imin,s,a);    % new partial sum
    s=Carry(c,s);
end 
```

With these preparations we can now compute 

```txt
>> s=EmultPrec(10,10)
s =
2 7 1 8 2 8 1 8 2 3
>> e=sprintf('%01d',s)
e =
2718281823 
```

To compute more digits we use 

```txt
>> s=EmultPrec(10,60); e=sprintf('%01d',s)
e =
271828182845904523536028747135266249775724709369995957496673 
```

Because of Rounding errors some of the last printed digits are not correct. We can check this by computing 10 more digits: 

```txt
>> s=EmultPrec(10,70); e=sprintf('%01d',s)
e =
2718281828459045235360287471352662497757247093699959574966967627724050 
```

So we see that the last two digits of s=EmultPrec(10,60) are affected by rounding errors. 

## Packing More Digits in One Array Element

The parameter c of EmultPrec controls how many digits are stored in one array element. If we change it to c=100 we work with two digits per array element and get 

```txt
>> s=EmultPrec(100,30); e=sprintf('%01d',s)
e =
27182818284594523536287471352662497757247936999595749646 
```

Note that the printed result is wrong! Zeros are missing, e.g. for the sequence after the 13th digit we get 5945 instead of 59045. We have to adjust the format to print 2 digits with leading zero if necessary: 

```txt
>> s=EmultPrec(100,30); e=sprintf('%02d',s)
e =
027182818284590452353602874713526624977572470936999595749646 
```

Now the result is correct. 

## 5.2 MATLAB-Elements Used in This Chapter

uint32: Convert to 32-bit unsigned integer. intArray = uint32(array) converts the elements of an array into unsigned 32-bit (4-byte) integers of class uint32. intArray: Array of class uint32. Values range from 0 to $2 ^ { 3 2 } - 1$ 

zeros: Create array of all zeros. 

X = zeros(sz) returns an array ofzeros where size vector sz defines size(X). For example, zeros([2 3]) returns a 2-by-3 matrix. 

X = zeros(1,3,‘uint32’) 

Create a 1-by-3 vector of zeros whose elements are 32-bit unsigned integers. 

idivide: Integer division with rounding option. 

C = idivide(A, B) is the same as A./B except that fractional quotients are rounded toward zero to the nearest integers. 

mod: Modulus after division. 

M = mod(X,Y) returns the modulus after division of X by Y. In general, if Y does not equal 0, M = mod(X,Y) returns $\mathrm { X \mathrm { ~ - ~ } \mathrm { n . ^ { * } Y } , }$ where n = floor(X./Y). 

sprintf: Format data into string str = sprintf(formatSpec,A1,...,An) formats the data in arrays A1,...,An according to formatSpec in column order, and returns the results to string str. 

## 5.3 Problems

For the following problems, make use of the functions we developed for computing Euler’s number e. 

1. Compute using multiple precision the powers of 2: 

$$
2 ^ {i}, \quad i = 1, 2, \ldots , 3 0 0.
$$

2. Write a program to compute factorials using multiple precision: 

$$
n!, \quad n = 1, 2, \dots , 2 0 0.
$$

3. Compute π to 1000 decimal digits. Use the relation by C. Størmer: 

$$
\pi = 2 4 \arctan {\frac {1}{8}} + 8 \arctan {\frac {1}{5 7}} + 4 \arctan {\frac {1}{2 3 9}}.
$$

## Hints:

Compute first a multiprecision arctan function using the Taylor-series (4.8) as proposed in Chap. 4: 

$$
\arctan x = \sum_ {k = 0} ^ {\infty} (- 1) ^ {k} \frac {x ^ {2 k + 1}}{2 k + 1} = x - \frac {x ^ {3}}{3} + \frac {x ^ {5}}{5} - \dots
$$

The above series is alternating so there is a danger of cancellation. However, since it is used only for $| x | < 1$ this is not much a concern. What we need is a new funtion Sub 

```matlab
function r=Sub(c,a,b)
% SUB computes r=a-b where a and b are multiprecision numbers
% with a>b. 
```

to subtract two multiprecision numbers. One has to be careful not to generate negative numbers, all intermediate results have to remain positive. 

To compute π we have to evaluate for some integer $p \ > \ 1$ the function arctan(1/p). When generating the next term after 

$$
t _ {k} = \frac {x ^ {2 k + 1}}{2 k + 1}
$$

for $x = 1 / p$ we have to form 

$$
t _ {k + 1} = t _ {k} / p ^ {2} / (2 k + 1).
$$

There is bug that one has to avoid: by dividing the last term twice by p and a third time by 2k 1 the variable imin is updated. For the next term we need to know the value of imin before the division by 2k 1! Otherwise we will get erroneous results when forming $t _ { k } / p ^ { 2 }$ 

In this chapter we shall develop a method to solve linear equations. Given a matrix A and a right hand side b 

$$
A = \left( \begin{array}{c c c c} a _ {1 1} & a _ {1 2} & \dots & a _ {1 n} \\ \vdots & \vdots & \ldots & \vdots \\ a _ {m 1} & a _ {m 2} & \dots & a _ {m n} \end{array} \right), \quad \boldsymbol {b} = \left( \begin{array}{c} b _ {1} \\ \vdots \\ b _ {m} \end{array} \right)
$$

then a solution of $A x \ = \ b$ is given in Matlab by $\mathtt { x } { = } \mathtt { A } \backslash \mathtt { b }$ . Notice that Matlab produces a solution for any values of n and m. The -operator is very powerful but to understand it one has to know what it computes. We shall explain here only the cases when $m = n$ and $m > n$ 

$m = n ;$ : We have as many equations as unknowns. If the matrix A is non-singular then the linear system has exactly one solution $x = A ^ { - 1 } b$ 

$m > n \colon$ The system is overdetermined, it has more equations than unknowns. In general there is no solution, the equations contradict themselves. A way to find a good “solution” was given by Carl Friedrich Gauss who invented the Least Squares Method. This method determines a solution vector x by minimizing the length of the residual $r = b - A x$ 

$$
\| \boldsymbol {r} \| _ {2} ^ {2} = \| \boldsymbol {b} - A \boldsymbol {x} \| _ {2} ^ {2} = \min.
$$

## 6.1 Gaussian Elimination and LU Decomposition

Given an $n \times n$ linear system, the usual way to compute a solution is by Gaussian elimination. In the first step the unknown $x _ { 1 }$ is eliminated from equations two to n, leaving a reduced $( n - 1 ) \times ( n - 1 )$ )-system containing only the unknowns $x _ { 2 } , \ldots , x _ { n }$ . Continuing the elimination steps we finally obtain an equation with the only unknown $x _ { n }$ The original system is thus transformed and reduced to a triangular system $U x = y ;$ 

$$
\left( \begin{array}{c c c c} u _ {1 1} & u _ {1 2} & \dots & u _ {1 n} \\ & u _ {2 2} & \dots & u _ {2 n} \\ & & \ddots & \vdots \\ & & & u _ {n n} \end{array} \right) \left( \begin{array}{c} x _ {1} \\ x _ {2} \\ \vdots \\ x _ {n} \end{array} \right) = \left( \begin{array}{c} y _ {1} \\ y _ {2} \\ \vdots \\ y _ {n} \end{array} \right)
$$

and the solution is easily computed by back-substitution. One can show that by this elimination process the matrix A is factorized in a product of a unit lower triangular matrix L and an upper triangular matrix $U !$ : 

$$
A = L U.
$$

The elimination process is mathematically equivalent with transforming the linear system by multiplying it from the left with the non-singular matrix $L ^ { - 1 }$ 

$$
A \boldsymbol {x} = \boldsymbol {b} \implies L ^ {- 1} A \boldsymbol {x} = L ^ {- 1} \boldsymbol {b} \iff U \boldsymbol {x} = \boldsymbol {y}.
$$

Things get a bit more complicated if the equation which should be used for eliminating $x _ { k }$ does not contain this variable. Then one has to permute the equations to continue the elimination process. This partial pivoting strategy is used when solving equations by the -operator. If no equation is found which contains $x _ { k }$ in the kth elimination step or if the coefficient of $x _ { k }$ is very small then the system is considered to be singular and a warning message is issued: 

```txt
Warning: Matrix is close to singular or badly scaled. Results may be inaccurate. RCOND = 4.800964e-18. 
```

The Matlab-function lu computes the LU-factorization of a matrix. We enter a $5 \times 5$ matrix: 

```asm
>> A = [12, 1, 2, 2, 10; 14 4 15 6 1
    2 8 14 14 13
    14 14 7 12 14
    9 14 12 14 10]
A =
12    1    2    2    10
14    4    15    6    1
2    8    14    14    13
14    14    7    12    14
9    14    12    14    10 
```

Notice that the elements on a row are separated by spaces or by a comma. A new row can either be started on the same line by inserting a semicolon or by typing it on a new line. Next we call the function lu: 

$$
\begin{array}{l l l l l l} \gg & [ L, U, P ] = l u (A) \\ L = & & & & & \\ & 1. 0 0 0 0 & 0 & 0 & 0 & 0 \\ & 0. 6 4 2 9 & 1. 0 0 0 0 & 0 & 0 & 0 \\ & 0. 8 5 7 1 & - 0. 2 1 2 5 & 1. 0 0 0 0 & 0 & 0 \\ & 0. 1 4 2 9 & 0. 6 5 0 0 & - 0. 9 9 7 0 & 1. 0 0 0 0 & 0 \\ & 1. 0 0 0 0 & 0. 8 7 5 0 & 0. 9 7 1 6 & - 0. 3 4 4 2 & 1. 0 0 0 0 \\ U = & & & & & \\ & 1 4. 0 0 0 0 & 4. 0 0 0 0 & 1 5. 0 0 0 0 & 6. 0 0 0 0 & 1. 0 0 0 0 \\ & 0 & 1 1. 4 2 8 6 & 2. 3 5 7 1 & 1 0. 1 4 2 9 & 9. 3 5 7 1 \\ & 0 & 0 & - 1 0. 3 5 6 2 & - 0. 9 8 7 5 & 1 1. 1 3 1 2 \\ & 0 & 0 & 0 & 5. 5 6 5 5 & 1 7. 8 7 2 7 \\ & 0 & 0 & 0 & 0 & 0.   {1}   {4}   {8}   {3} \\ P = & & & & \\ & \begin{array}{c c c c c c} \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \\ \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \end{array} \\ P = & \\ & \begin{array}{c c c c c c} \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \hline \\ \hline \hline \hline \hline \hbar^ {2} = [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ U, U, P ] = l u (A) \\ [ U, U, P ] = l u (A) \\ [ U, U, P ] = l u (A) \\ [ U, U, P ] = l u (A) \\ [ U, U, P ] = l u (A) \\ [ U, U, P ] = l u (A) \\ [ U, U, P ] = l u (A) \\ [ U, I, U, P ] = l u (A) \\ [ U, I, U, P ] = l u (A) \\ [ U, I, U, P ] = l u (A) \\ [ U, I, U, P ] = l u (A) \\ [ U, I, U, P ] = l u (A) \\ [ U, I, U, P ] = l u (A) \\ [ U, I, U, S ] = l u (A) \\ [ U, I, U, P ] = l u (A) \\ [ U, I, U, P ] = l u (A) \\ [ U, I, U, S ] = l u (A) \\ [ U, I, U, P ] = l u (A) \\ [ U, I, U, P ] = l u (A) \\ [ U, I, U, S ] = l w h e r t h e r m a x i n g e r e d o f t h e r m a x i n g e r e d o f t h e r m a x i n g e r e d o f t h e r m a x i n g e r e d o f t h e r m a x i n g e r e d o f t h e r m a x i n g e r e d o f t h e r m a x i n g e r e d o f t h e t h e r m a x i n g e r e d o f t h e r m a x i n g e r e d o f t h e t h e r m a x i n g e r e d o f t h e t h e r m a x i n g e r e d o f t h e t h e t h e r m a x i n g e r e d o f t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e t h e T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T H T W E R M O N D O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E G W E R M O N D O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F O R E F G W E R M O N D O R E F G W E R M O N D O R E F G W E R M O N D O R E F G W E R M O N D O R E F G W E R M O N D O R E F G W E R M O N D O R E F G W E R M O N D O R E F G W E R M O N D O R E F G W E R M O N D O R E G W W E R M O N D O R E G W W E R M O N D O R E G W W E R M O N D O R E G W W E R M O N D O R E G W W W E R M O N D O R E G W W W E R M O N D O R E G W W W W E R M O N D O R E G W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W W Y K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K K C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B C A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B S S A B s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a bs a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s a b s y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k yk y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y k y z , \\ & [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ L, U, P ] = l u (A) \\ [ I, U, P ] = l u (A) \\ [ I, U, P ] = l u (A) \\ [ I, U, P ] = l u (A) \\ [ I, U, P ] = l u (A) \\ [ I, U, P ] = l u (A) \\ [ I, U, P ] = l u (A) \\ [ I, U, P ] = l u (A) \\ [ I, I, U ] = l u (A) \\ [ I, I, U ] = l u (A) \\ [ I, I, U ] = l u (A) \\ [ I, I, U ] = l u (A) \\ [ I, I, U ] = l u (A) \\ [ I, I, U ] = l u (A) \\ [ I, I, U ] = l u (A) \\ [ I, I, U ] ^ {\text {if}} \\ [ I, I, U ] ^ {\text {of}} \\ [ I, I, U ] ^ {\text {of}} \\ [ I, I, U ] ^ {\text {of}} \\ [ I, I, U ] ^ {\text {of}} \\ [ I, I, U ] ^ {\text {of}} \\ [ I, I, U ] ^ {\text {of}} \\ [ I, I, U ] ^ {\text {of}} \\ [ I, I, U ] ^ {\text {of}}; \\ [ I, I, U ] ^ {\text {of}}; \\ [ I, I, U ] ^ {\text {of}}; \\ [ I, I, U ] ^ {\text {of}}; \\ [ I, I, U ] ^ {\text {of}}; \\ [ I, I, U ] ^ {\text {of}}; \\ [ I, I, U ] ^ {\text {of}}; \\ [ I, I, U ] ^ {T} ; \\ [ I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I , I | .\
$$

We obtain two triangular matrices L and U and a permutation matrix P. They are related by 

$$
P A = L U.
$$

Let’s check this and compute LU and P A: 

$$
\begin{array}{l l l l l l} \text {>> L*U} \\ \text {ans =} \\ 1 4. 0 0 0 0 & 4. 0 0 0 0 & 1 5. 0 0 0 0 & 6. 0 0 0 0 & 1. 0 0 0 0 \\ 9. 0 0 0 0 & 1 4. 0 0 0 0 & 1 2. 0 0 0 0 & 1 4. 0 0 0 0 & 1 0. 0 0 0 0 \\ 1 2. 0 0 0 0 & 1. 0 0 0 0 & 2. 0 0 0 0 & 2. 0 0 0 0 & 1 0. 0 0 0 0 \\ 2. 0 0 0 0 & 8. 0 0 0 0 & 1 4. 0 0 0 0 & 1 4. 0 0 0 0 & 1 3. 0 0 0 0 \\ 1 4. 0 0 0 0 & 1 4. 0 0 0 0 & 7. 0 0 0 0 & 1 2. 0 0 0 0 & 1 4. 0 0 0 0 \\ \text {>> P*A} \\ \text {ans =} \\ \text {14} & \text {4} & \text {15} & \text {6} & \text {1} \\ \text {9} & \text {14} & \text {12} & \text {14} & \text {10} \\ \text {12} & \text {1} & \text {2} & \text {2} & \text {10} \\ \text {2} & \text {8} & \text {14} & \text {14} & \text {13} \\ \text {14} & \text {14} & \text {7} & \text {12} & \text {14} \end{array}
$$

As expected, the product LU is equal to the permuted matrix A. Consider now a vector for the right hand side: 

```txt
>> y=P*b
y =
2
5
1
3
4
>> y=L\y
y =
2.0000
3.7143
0.0750
0.3748
-1.1939
>> x=U\y
x =
5.4751
-13.7880
-11.1287
25.9130
-8.0482 
```

```coffeescript
>> b=[1:5] '
b =
1
2
3
4
5 
```

Notice that 1:5 is the abbreviation for the vector [1,2,3,4,5] and the apostrophe transposes the vector to become a column vector. The solution of Ax b is given by x=A b. 

```txt
>> x=A\b
x =
5.4751
-13.7880
-11.1287
25.9130
-8.0482 
```

The -operator computes in this case first a LU-decomposition and then obtains the solution by solving Ly Pb by forward-substitution followed by solving Ux y with backward-substitution. We can check this with the following statements. 

## 6.2 Elimination with Givens-Rotations

In this section we present another elimination algorithm which is computationally more expensive but simpler to program and which can be used also for least squares problem. 

We proceed as follow to eliminate in the ith step the unknown $x _ { i }$ in equations $i + 1$ to n. Let 

$$
\begin{array}{c} (i): a _ {i i} x _ {i} + \ldots + a _ {i n} x _ {n} = b _ {i} \\ \vdots \qquad \qquad \qquad \vdots \\ (k): a _ {k i} x _ {i} + \ldots + a _ {k n} x _ {n} = b _ {k} \\ \vdots \qquad \qquad \qquad \vdots \\ (n): a _ {n i} x _ {i} + \ldots + a _ {n n} x _ {n} = b _ {n} \end{array}\tag{6.1}
$$

be the reduced system. To eliminate $x _ { i }$ in equation (k) we multiply equation (i) by sin α and equation (k) by cos α and replace equation (k) by the linear combination 

$$
(k) _ {n e w} = - \sin \alpha \cdot (i) + \cos \alpha \cdot (k),\tag{6.2}
$$

where we have chosen α so, that 

$$
a _ {k i} ^ {n e w} = - \sin \alpha \cdot a _ {i i} + \cos \alpha \cdot a _ {k i} = 0.\tag{6.3}
$$

No elimination is necessary if $a _ { k i } = 0$ , otherwise we can use Eq. (6.3) to compute 

$$
\cot \alpha = \frac {a _ {i i}}{a _ {k i}}\tag{6.4}
$$

and get 

$$
\begin{array}{l} \cot = A (i, i) / A (k, i); \\ \text {si} = 1 / s q r t (1 + \cot * \cot); \\ \text {co} = \text {si} * \cot . \end{array}\tag{6.5}
$$

In this elimination we do not only replace equation (k) but seemingly unnecessarily also equation (i) by 

$$
(i) _ {n e w} = \cos \alpha \cdot (i) + \sin \alpha \cdot (k).\tag{6.6}
$$

Doing so we do not need to permute the equations as with Gaussian Elimination. This is done automatically. We illustrate this for the case if $a _ { i i } = 0$ and $a _ { k i } \neq 0$ . Here we obtain cot $\alpha = 0$ thus sin $\alpha = 1$ and cos $\alpha = 0$ . Computing the two Eqs. (6.2) and (6.6) results in just permuting them! 

The Givens Elimination algorithm is easy to program since we can use Matlab’s vector-operations. To multiply the ith row of the matrix A by a factor $\scriptstyle \mathtt { C O } = \cos ( \alpha )$ 

$$
\cos (\alpha) [ a _ {i 1}, a _ {i, 2}, \dots , a _ {i n} ]
$$

we use the statement 

```txt
CO*A(i, :) 
```

The colon notation is an abbreviation for A(i,1:n) or more general A(i,1:end). The variable end serves as the last index in an indexing expression. Thus the new ith row of the matrix becomes 

$$
A (i,:) = C O * A (i,:) + S i * A (k,:)
$$

By doing so we overwrite the ith row of A with new elements. This makes it impossible to compute the new kth row since we need the old values of the ith row! We have to save the new row first in a auxiliary variable h and assign it later: 

```matlab
A(i, i) = A(i, i) * co + A(k, i) * si;
h = A(i, i + 1:n) * co + A(k, i + 1:n) * si;
A(k, i + 1:n) = -A(i, i + 1:n) * si + A(k, i + 1:n) * co;
A(i, i + 1:n) = h; 
```

Since A(k,i) becomes zero we do not compute it. Also we do not use A(i,:) but rather A(i,i+1:n) since the elements on the row before the diagonal are zero and don’t have to be processed. 

We propose here a more elegant solution without auxiliary variable. The Givens elimination is performed by transforming the two rows with a rotation matrix 

$$
\left( \begin{array}{c c} c & s \\ - s & c \end{array} \right) \left( \begin{array}{c c c c} A (i, i) & A (i, i + 1) & \ldots & A (i, n) \\ A (k, i) & A (k, i + 1) & \ldots & A (k, n) \end{array} \right)
$$

An assignment statement in Matlab cannot have two results. But by using the expression A(i:k-i:k,i+1:n) we can change both rows of A in one assignment with one result. Thus we get the compact assignments 

```txt
A(i,i)=A(i,i)*co+A(k,i)*si;
S=[co,si;-si,co];
A(i:k-i:k,i+1:n)=S*A(i:k-i:k,i+1:n); 
```

In the same way we also change the right hand side. Putting all together we obtain the function: 

## 6.2 Elimination with Givens-Rotations

```matlab
function x=EliminationGivens(A,b);
% ELIMINATIONGIVENS solves a linear system using Givens-rotations
% x=EliminationGivens(A,b) solves Ax=b using Givens-rotations.
[m,n]=size(A);
for i=1:n
    for k=i+1:m
    if A(k,i)~=0
    cot=A(i,i)/A(k,i); % rotation angle
    si=1/sqrt(1+cot^2); co=si*cot;
    A(i,i)=A(i,i)*co+A(k,i)*si;
    S=[co,si;-si,co];
    A(i:k-i:k,i+1:n)=S*A(i:k-i:k,i+1:n);
    b(i:k-i:k)=S*b(i:k-i:k);
    end
    end;
    if A(i,i)==0
    error('Matrix is rank deficient');
    end;
end
x=zeros(n,1);
for k=n:-1:1 % backsubstitution
    x(k)=(b(k)-A(k,k+1:n)*x(k+1:n))/A(k,k);
end
x=x(:); 
```

The transformation of $A x \ = \ b$ to the reduced system $U x \ = \ y$ is done this time with Givens rotations. These rotation matrices are not only non-singular but also orthogonal (a matrix Q is orthogonal if $Q ^ { \top } Q \ : = \ : I )$ . Transformations with orthogonal matrices leave the length invariant: 

$$
z = Q r \implies \| z \| _ {2} ^ {2} = z ^ {\top} z = (Q r) ^ {\top} Q r = r ^ {\top} Q ^ {\top} Q r = r ^ {\top} r = \| r \| _ {2} ^ {2}.
$$

Therefore the solution of minimizing the length of the residual $r = b - A x$ does not change of we multiply the system by an orthogonal matrix: 

$$
A \boldsymbol {x} = \boldsymbol {b} \iff Q ^ {\top} A \boldsymbol {x} = Q ^ {\top} \boldsymbol {b}.
$$

With Givens elimination we therefore can solve linear n n-systems and also overdetermined systems in the least square sense. The Matlab -operator solves least squares systems using orthogonal transformations. 

$$
y = a t + \frac {b}{t} + c \sqrt {t}
$$

We illustrate this with the following example. We wish to fit a function of the form 

to the points 

<table><tr><td>t</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td></tr><tr><td>y</td><td>2.1</td><td>1.6</td><td>1.9</td><td>2.5</td><td>3.1</td></tr></table>

Inserting the points we get the linear system 

$$
\left( \begin{array}{c c c} 1 & 1 & 1 \\ 2 & 1 / 2 & \sqrt {2} \\ 3 & 1 / 3 & \sqrt {3} \\ 4 & 1 / 4 & \sqrt {4} \\ 5 & 1 / 5 & \sqrt {5} \end{array} \right) \left( \begin{array}{c} a \\ b \\ c \end{array} \right) = \left( \begin{array}{c} 2. 1 \\ 1. 6 \\ 1. 9 \\ 2. 5 \\ 3. 1 \end{array} \right)
$$

We get with GivensElimination the same result as with Matlab’s -operator: 

```matlab
% file CurveFit.m
A=[ 1 1 1
    2 1/2 sqrt(2)
    3 1/3 sqrt(3)
    4 1/4 sqrt(4)
    5 1/5 sqrt(5)];
b=[ 2.1 1.6 1.9 2.5 3.1]';
t=[1:5]';
plot(t,b,'o')
hold
x=EliminationGivens(A,b)
y=A\b
pause % compare x with y, they are the same
xx=[1:0.1:5];
yy=y(1).*xx+y(2)./xx+y(3).*sqrt(xx);
plot(xx,yy)

>> CurveFit
x =
    1.0040
    2.1367
    -1.0424
y =
    1.0040
    2.1367
    -1.0424 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/ec6e1a484f1222f8c5aab019e4a6b802a3636d3fb0e5838e35581ad82d441811.jpg)


## 6.3 MATLAB-Elements Used in This Chapter

mldivide, (backslash-operator) Solve systems of linear equations Ax = B for x 

x = A B solves the system of linear equations $\mathbf { A } ^ { * } \mathbf { X } = \mathbf { B }$ . The matrices A and B must have the same number of rows. MATLAB displays a warning message ifA is badly scaled or nearly singular, but performs the calculation regardless. 

## : Colon

```txt
J:K is the same as [J, J+1, ..., K].
J:K is empty if J>K.
J:D:K is the same as [J, J+D, ..., J+m*D] where m=fix((K-J)/D).
J:D:K is empty if D == 0, if D>0 and J>K, or if D<0 and J<K.
COLON(J,K) is the same as J:K and COLON(J,D,K) is the same as J:D:K.
The colon notation can be used to pick out selected rows, columns and elements of vectors, matrices, and arrays. A(:) is all the elements of A, regarded as a single column. On the left side of an assignment statement, A(:) fills A, preserving its shape from before. A(:,J) is the J-th column of A. A(J:K) is [A(J),A(J+1),...,A(K)]. A(:,J:K) is [A(:,J),A(:,J+1),...,A(:,K)] and so on. 
```

lu: 

[L,U,P] = LU(A) returns unit lower triangular matrix L, upper triangular matrix U, and permutation matrix P so that $\begin{array} { r } { \mathrm { \Delta p } _ { \star \mathrm { A } } ~ = ~ \mathrm { L } { \star \mathrm { U } } } \end{array}$ 

## planerot: Givens plane rotation

[G,y] = planerot(x) where x is a 2-component column vector, returns a 2-by-2 orthogonal matrix G so that $\mathbf { y } = \mathbf { G } ^ { * } \mathbf { x }$ has $\mathbf { y } ( 2 ) = 0$ 

## ’ ctranspose: Complex conjugate transpose

b = a’ computes the complex conjugate transpose of matrix a and returns the result in b. 

The following commands are used in the problem section. 

```erlang
>> format short e, format compact
>> n=5; A=invhilb(n), b=eye(n,1) 
```

pause: Halt execution temporarily 

pause, by itself, causes the currently executing function to stop and wait for you to press any key before continuing. Pausing must be enabled for this to take effect. (See pause on, below.) Pause without arguments also blocks execution of Simulink models, but not repainting of them. 

pause(n) pauses execution for n seconds before continuing, where n is any nonnegative real number. Pausing must be enabled for this to take effect. 

tril: Lower triangular part of matrix 

L = tril(X) returns the lower triangular part of X. 

L = tril(X,k) returns the elements on and below the kth diagonal of X. 

k = 0 is the main diagonal, k > 0 is above the main diagonal, and k < 0 is below the main diagonal. 

triu: Upper triangular part of matrix 

U = triu(X) returns the upper triangular part of X. 

U = triu(X,k) returns the element on and above the kth diagonal of X. 

k = 0 is the main diagonal, k > 0 is above the main diagonal, and k < 0 is below the main diagonal. 

diag: Create diagonal matrix or get diagonal elements of matrix 

D = diag(v) returns a square diagonal matrix with the elements of vector v on the main diagonal. 

D = diag(v,k) places the elements of vector v on the kth diagonal. k 0 represents the main diagonal, k > 0 is above the main diagonal, and k < 0 is below the main diagonal. 

x = diag(A) returns a column vector of the main diagonal elements of A. 

x = diag(A,k) returns a column vector of the elements on the kth diagonal of A. 

## 6.4 Problems

1. LU-decomposition Consider the linear system Ax b defined by the matrix (a) Apply Gaussian Elimination (without pivoting) to reduce the system to Ux y 

```matlab
for j=1:n-1 % Elimination
    for k=j+1:n
    fak=A(k,j)/A(j,j);
    A(k,j:n)=A(k,j:n)-fak*A(j,j:n);
    b(k)=b(k)-fak*b(j);
    end
end 
```

Watch the elimination process by displaying the matrix and the right hand side after each elimination step. Use the pause statement to stop execution. 

(b) Next store the factors fak instead of the zeros you introduce by eliminating x <sub>j</sub> : 

```matlab
for j=1:n-1 % Elimination
    for k=j+1:n
    fak=A(k,j)/A(j,j);
    A(k,j)=fak; % store factors instead zeros
    A(k,j+1:n)=A(k,j+1:n)-fak*A(j,j+1:n);
    end
end 
```

Now use the commands triu, tril, diag to extract L and U from A and verify that indeed LU A. 

2. Replace the computation of the rotation matrix S in our function 

EliminationGivens by the Matlab-function planerot. Convince yourself that you get the same results with the modified function by solving the curve fitting example again. 

3. Determine the parameters a and b such that the function $f ( x ) = a e ^ { b x }$ fits the following data 

<table><tr><td>x</td><td>30.0</td><td>64.5</td><td>74.5</td><td>86.7</td><td>94.5</td><td>98.9</td></tr><tr><td>y</td><td>4</td><td>18</td><td>29</td><td>51</td><td>73</td><td>90</td></tr></table>

Plot the points and the fitted function. 

Hint: If you fit log f(x) the problem becomes very easy! 

4. The following statistics lists the population of Shanghai since 1953: 

<table><tr><td>year</td><td>in million</td></tr><tr><td>1953</td><td>6.2044</td></tr><tr><td>1964</td><td>10.8165</td></tr><tr><td>1982</td><td>11.8597</td></tr><tr><td>1990</td><td>13.3419</td></tr><tr><td>2000</td><td>16.4077</td></tr><tr><td>2010</td><td>23.0192</td></tr></table>

Fit a polynomial through these data and predict the population for 2016 and 2020. Plot your results. 

5. Fitting ofcircles. We are given the measured points $( \xi _ { i } , \eta _ { i } )$ 

<table><tr><td>ξ</td><td>0.7</td><td>3.3</td><td>5.6</td><td>7.5</td><td>6.4</td><td>4.4</td><td>0.3</td><td>-1.1</td></tr><tr><td>η</td><td>4.0</td><td>4.7</td><td>4.0</td><td>1.3</td><td>-1.1</td><td>-3.0</td><td>-2.5</td><td>1.3</td></tr></table>

Find the center $( c _ { 1 } , c _ { 2 } )$ and the radius r of a circle $( x - c _ { 1 } ) ^ { 2 } + ( y - c _ { 2 } ) ^ { 2 } = r ^ { 2 }$ that approximate the points as well as possible. Consider the algebraicfit: Rearrange the equation of the circle as 

$$
2 c _ {1} x + 2 c _ {2} y + r ^ {2} - c _ {1} ^ {2} - c _ {2} ^ {2} = x ^ {2} + y ^ {2}.\tag{6.7}
$$

With $w = r ^ { 2 } - c _ { 1 } ^ { 2 } - c _ { 2 } ^ { 2 }$ , we obtain with (6.7) for each measured point a linear equation for the unknowns $c _ { 1 } , c _ { 2 }$ and w. 

Write a function function drawcircle(C,r) to plot a circle with center $\left( \textrm { C } ( 1 ) , \textrm { C } ( 2 ) \ \right)$ ) and radius r. 

Computer the center and the radius and plot the given points and the fitted circle. 

6. Seven dwarfs are sitting around a table. Each one has a cup. The cups contain milk, all together a total of 3 liter. One of the dwarfs starts distributing his milk evenly over all cups. After he has finished his right neighbor does the same. Clockwise the next dwarfs proceed distributing their milk. After the 7th dwarf has distributed his milk, there is in each cup as much milk as at the beginning. How much milk was initially in each cup? 

Hint: Let $\pmb { x } = ( x _ { 1 } , x _ { 2 } , \ldots , x _ { 7 } ) ^ { \top }$ be the initial milk distribution. Thus $\textstyle \sum _ { j = 1 } ^ { 7 } x _ { j } =$ 3. Simulate the distributing of milk as matrix-vector Operation: 

$$
\pmb {x} ^ {(1)} = T _ {1} \pmb {x}.
$$

After 7 distributions you obtain $\mathbf { x } ^ { ( 7 ) } = \mathbf { x }$ and thus 

$$
\boldsymbol {x} = T _ {7} T _ {6} \dots T _ {1} \boldsymbol {x}
$$

or $( A - I ) \mathbf { { x } } \ = \ 0$ where $A ~ = ~ T _ { 7 } T _ { 6 } \cdot \cdot \cdot T _ { 1 }$ . Add to this homogeneous system the equation $\textstyle \sum _ { j = 1 } ^ { 7 } x _ { j } = 3$ and solve the system using our function EliminationGivens. Compare the results you get with those when using Matlab’s -operator. 

## 6.4 Problems

7. The following sections were measured on the street $\overline { { A D } }$ depicted in Fig. 6.1. 

$$
\mathrm{AD} = 8 9 \mathrm{m}, \mathrm{AC} = 6 7 \mathrm{m}, \mathrm{BD} = 5 3 \mathrm{m}, \mathrm{AB} = 3 5 \mathrm{mandCD} = 2 0 \mathrm{m}
$$

Balance out the measured sections using the least squares method. 

<table><tr><td>A</td><td>B</td><td>C</td><td>D</td></tr></table>


Fig. 6.1 Street


## 7.1 Introduction

Recursion is a powerful concept in computer science. The basic idea is that the solution of a problem often can be reduced to solving some smaller instances of the same problem. Recursive solutions can be applied to many problems, one well known strategy is called divide and conquer. 

A function is sometimes defined recursively. For instance the factorial, the function 

$$
f (n) = n! = 1 \times 2 \times 3 \times \dots \times n
$$

can be defined recursively by 

$$
\begin{array}{c} 0! = 1 \\ f (n) = n \times f (n - 1), \quad n > 0. \end{array}
$$

In Matlab we could just use the expression prod(1:n) or factorial(n) to compute this function. To show the concept of recursion we program the function 

```matlab
function f=Factorial(n)
if n==0,
    f=1;
else
    f=n*Factorial(n-1);
end 
```

The function f is calling itself in its definition. This is called a recursive function. A recursion that contains only one single self-reference is known as single recursion, while a recursion that contains multiple self-references is known as multiple recursion. A single recursion can be programmed easily as an iteration, which is simpler and more efficient. For our factorial example we would get 

```matlab
function f=FactorialIteration(n)
f=1;
for k=1:n
    f=k*f;
end 
```

We get for all variants the same 

```txt
>> n=10;
>> [prod(1:n), factorial(n), FactorialIteration(n), Factorial(n)]
ans =
3628800 3628800 3628800 3628800 
```

## 7.2 Laplace Expansion for Determinants

The determinant of a matrix A can be computed using the Laplace Expansion. For each row i we have 

$$
\det (A) = \sum_ {j = 1} ^ {n} a _ {i j} (- 1) ^ {i + j} \det (M _ {i j}),\tag{7.1}
$$

where $M _ { i j }$ denotes the $( n \mathrm { ~ - ~ } 1 ) \times ( n \mathrm { ~ - ~ } 1 )$ submatrix obtained by deleting row i and column j of the matrix A. Thus computing the determinant of A is reduced to compute n smaller determinants of the submatrices $M _ { i j }$ . Instead of expanding the determinant as in (7.1) along a row, we can also use an expansion along a column. 

The following Matlab program is an example for multiple recursion, it computes a determinant using the Laplace Expansion for the first row: 

```matlab
function d=DetLaplace(A);
% DETLAPLACE determinant using Laplace expansion
%    d=DetLaplace(A); computes the determinant d of the matrix A
% using the Laplace expansion for the first row.

n=length(A);
if n==1;
    d=A(1,1);
else 
    d=0; v=1;
    for j=1:n 
    M1j=[A(2:n,1:j-1) A(2:n,j+1:n)];
    d=d+v*A(1,j)*DetLaplace(M1j);
    v=-v;
    end 
end 
```

In Matlab the function det computes the determinant in a more efficient way (using Gaussian Elimination) than our recursive function. The following examples show both results: 

## 7.2 Laplace Expansion for Determinants

```txt
for n=4:9
    A=rand(n);
    [det(A) DetLaplace(A)]
end

ans =
    0.128257928707307    0.128257928707307
ans =
    -0.084250098064663    -0.084250098064664
ans =
    -0.181256419130385    -0.181256419130385
ans =
    -0.022309977397375    -0.022309977397376
ans =
    -0.006338537112776    -0.006338537112776
ans =
    -0.008692776468285    -0.008692776468285 
```

The results are the same, the only difference is that Laplace’s formula needs much more operations and thus uses much more execution time that det. However, if we replace rand by hilb, the matrices are Hilbert matrices which are ill-conditioned, we get 

```matlab
for n=4:9
    A=hilb(n);
    [det(A) DetLaplace(A)]
end

ans =
    1.0e-06 *
    0.165343915343926    0.165343915343319
ans =
    1.0e-11 *
    0.374929513251423    0.374929513075645
ans =
    1.0e-17 *
    0.536729988684877    0.536730023323187
ans =
    1.0e-24 *
    0.483580261909806    0.483085292821939
ans =
    1.0e-30 *
    0.002737050274535   -0.355714248182654
ans =
    1.0e-35 *
    0.000000097202790    0.315086992638140 
```

This time the results of det are much more accurate than those with Laplace’s Expansion. Thus in summary, Laplace’s expansion is mathematically interesting and can be implemented recursively. It is, however, computationally much more expensive and numerically a disaster. 

## 7.3 Hilbert Curves

Hilbert curves are space filling curves. We follow here the derivation given in [13]. The basic elements for the construction are 4 “cups”. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/d839ed19722e3de063c15be67ba19817f66bece3519fa3d9f508cd122e16cca2.jpg)


a 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/365d65d30e978633ad6a026546cc9fa7ac0161c6997bcecbff11ddcf6a26103e.jpg)


b 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/abc9cc63474382ba52efd7632dfe60c3ce54bf1998dd99f1ed80041c45e4bb91.jpg)


c 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/b3eb1b651d330c4bfbf1d8c83c4f966511bc02e8b867a47daf9a357cc6176928.jpg)


d 

The next refinement of a is the curve $a _ { 2 }$ which is 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/509cda6d249a38836cf9f84cb7c435954844a3e66ba9089464893cdb180742f8.jpg)


It has been constructed by attaching a smaller d-cup to point A, the upper right of a, then moving a step h from point B to C to the left to place a small a-cup. Then moving down from point D to E again by a step h and placing another a-cup. Finally moving from F to $G$ another step h to the right and placing a b-cup. We wish to plot the resulting Hilbert curve, so we need to plot the segments BC, DE and FG. We thus get the function 

```matlab
function a(i);
global x y h;
if i > 0,
    d(i - 1); plot([x - h, x], [y, y]); x = x - h;
    a(i - 1); plot([x, x], [y - h, y]); y = y - h;
    a(i - 1); plot([x, x + h], [y, y]); x = x + h;
    b(i - 1);
end 
```

## 7.3 Hilbert Curves

The above curve is the result for i 2. Symbolically we write for the construction 

$$
a _ {2}: d \gets a \downarrow a \rightarrow b
$$

The coordinates of the current point on the curve are given by the global variables (x, y). The current step size h is also a global variable. 

Similarly we get for the d-cup starting from the upper right corner: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/bb4a27ba1ecbb11a5a94815291f04fd4b0d14ac70dea3dd2ebad24bdc0c5b596.jpg)



<sup>d</sup>2 <sup>: a d d c</sup>


An finally for b and c starting from the lower left corner: 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/5a3d7f9e0d928fe57193cdc11887899e12ece7eb601367a3799d36e547b9855b.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/1a77c723d7f59075bba159dba91b9f5d44cbde8fad593d071c074d6417e63e08.jpg)



<sup>c</sup>2 <sup>: b c c d</sup>


We program the 4 cases: 

```matlab
function a(i);
global x y h;
if i > 0,
d(i-1); plot([x-h, x], [y, y]); x = x - h;
a(i-1); plot([x, x], [y - h, y]); y = y - h;
a(i-1); plot([x, x + h], [y, y]); x = x + h;
b(i-1);
end

function b(i);
global x y h;
if i > 0,
c(i-1); plot([x, x], [y, y + h]); y = y + h;
b(i-1); plot([x, x + h], [y, y]); x = x + h;
b(i-1); plot([x, x], [y - h, y]); y = y - h;
a(i-1);
end 
```

```matlab
function c(i);
global x y h;
if i>0,
    b(i-1); plot([x,x+h],[y,y]); x=x+h;
    c(i-1); plot([x,x],[y,y+h]); y=y+h;
    c(i-1); plot([x-h,x],[y,y]); x=x-h;
    d(i-1);
end

function d(i);
global x y h;
if i>0,
    a(i-1); plot([x,x],[y-h,y]); y=y-h;
    d(i-1); plot([x-h,x],[y,y]); x=x-h;
    d(i-1); plot([x,x],[y,y+h]); y=y+h;
    c(i-1);
end 
```

Notice that these four functions are highly multiple recursive. Each one calls itself and two of the other functions. 

In the main program h1.m we need to define n and call a(n): 

```matlab
global x y h;
clf
axis([-600,800, -600, 800])
axis square
hold
x=600; y=600;
n=input('Hilbert Curve n=?')
h0=1024;
h=h0/2^n; % scaling to fill same square
a(n) 
```

The result for n 3 is 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/123cd5e949cb1ac859a268c97d1dd8e3b60b2790dfa018d8692d454c4cf7609f.jpg)


It is fun to watch the curve being plotted. For this we need to add the Matlabcommand drawnow while the curve is generated. We add this command to the function a.m: 

```matlab
function a(i);
global x y h
if i > 0,
    d(i - 1); plot([x - h, x], [y, y]); x = x - h;
    a(i - 1); plot([x, x], [y - h, y]); y = y - h;
    a(i - 1); plot([x, x + h], [y, y]); x = x + h;
    b(i - 1);
drawnow;
end 
```

Run now the main program again for n 6 and watch the curve being plotted! 

## 7.4 Quicksort

Quicksort is a ingenious sorting algorithm developed by Tony Hoare using recursion. Given a vector of numbers 

$$
\boldsymbol {a} = (a _ {1}, a _ {2}, \dots , a _ {n})
$$

we want to sort them in ascending order. We split the vector in two sets by choosing some element in the middle: 

$$
x = a (m) \text {where} m = \operatorname{round} ((1 + n) / 2)
$$

We then get two sets which are separated by x: 

$$
\{a _ {1}, \ldots , a _ {m - 1} \}, x, \{a _ {m + 1}, \ldots , a _ {n} \}.
$$

Now we scan the elements of the first set and search for an element $a _ { i } \geq x$ . Then we scan the elements of the second set and look for an element $a _ { j } \leq x$ . If we are successful, we swap $a _ { i }$ with $a _ { j }$ . We continue this way until the first set contains only numbers smaller than x and the second set only numbers larger than x. Then we apply the same procedure recursively and independently to the two sets. 

The following function Sorting generates first n random numbers and prints them as bar plot. 

```matlab
function Sorting(n)
global a
format short
a=rand(1,n);
clf, bar(a), pause
quick(1,n)
a 
```

Then it calls the recursive function quick: 

```matlab
function quick(left,right)
% QUICK quicksort
% quick(left,right) sorts the numbers a(left), ..., a(right) of the
% global array a in ascending order.
global a;
mid=round((left+right)/2); % choose middle element
i=left; j=right; x=a(mid); % sort a(i) ... a(j)
while i<=j
    while a(i)<x, i=i+1; end % search left for a(i)>=x
    while x<a(j), j=j-1; end % search right for a(j)<=x
    if i<=j % swap if found
    u=a(i); a(i)=a(j); a(j)=u;
    i=i+1; j=j-1; % advance indices
% bar(a); pause(0.01) % to show the process
end
end
if left<j, quick(left,j); end % sort the two sets
if i<right, quick(i,right); end % recursively 
```

When two elements are swapped we plot the array a and wait 0.01 s. This allows to visualize the quick-sort algorithm. Run the program for n 100 and watch how the numbers are sorted. In a parallel environment the sorting of the two subsets could be computed independently. 

## 7.5 MATLAB-Elements Used in This Chapter

prod: Product of array elements If A is a vector, then prod(A) returns the product of the elements. If A is a nonempty matrix, then prod(A) treats the columns of A as vectors and returns a row vector of the products of each column. 

factorial: Factorial of input f = factorial(n) returns the product of all positive integers less than or equal to n, where n is a nonnegative integer value. If n is an array, then f contains the factorial of each value of n. The data type and size of f is the same as that of n. 

det: Matrix determinant 

rand: Uniformly distributed pseudorandom numbers r = rand returns a pseudorandom scalar drawn from the standard uniform distribution on the open interval (0, 1). 

hilb: Hilbert matrix The Hilbert matrix is a notable example of a poorly conditioned matrix. The elements of the Hilbert matrices are H(i,j) = 1/(i + j 1). 

global: Declare global variables 

global X Y Z defines X, Y, and Z as global in scope. 

Ordinarily, each Matlab function has its own local variables, which are separate from those of other functions, and from those of the base workspace. However, if several functions, and possibly the base workspace, all declare a particular name as global, they all share a single copy of that variable. Any assignment to that variable, in any function, is available to all the functions declaring it global. 

drawnow: Update figure window and execute pending callbacks drawnow causes figure windows and their children to update. Any callbacks generated by user actions (for example, mouse or key presses, button clicks, and so on) are executed before drawnow returns. 

Use drawnow in animation loops to update the figure during function execution and to update graphical user interfaces. 

bar: Bar graph 

bar(Y) draws one bar for each element in Y. 

tic, toc: stopwatch timer 

tic starts a stopwatch timer to measure performance. The function records the internal time at execution of the tic command. Display the elapsed time with the toc function. 

## 7.6 Problems

1. Cramer’s Rule for solving systems of linear equations. This rule is often used when solving small $( n \leq 3 )$ systems of linear equations by hand. 

Write a function x=Cramer $( \mathtt { A } , \mathtt { b } )$ which solves a linear system $A { \boldsymbol { \mathbf { \mathit { x } } } } = \mathbf { \boldsymbol { \mathbf { b } } }$ using Cramer’s rule. For det $( A ) \neq 0$ , the linear system has the unique solution 

$$
x _ {i} = \frac {\det (A _ {i})}{\det (A)}, \quad i = 1, 2, \dots , n,\tag{7.2}
$$

where $A _ { i }$ is the matrix obtained from A by replacing column $\pmb { a } : i$ by b. Use the function DetLaplace to compute the determinants. 

Test your program by generating a linear system with known solution. 

2. Selection Sort versus Quick Sort. 

The idea of selection sort is to find the minimum value in the given array and then swaps it with the value in the first position. By repeating this for the remaining elements the array is sorted. 

(a) Write a (non-recursive) function a=SelectSort(a) which implements the Selection Sort. Show the process using bar and pause as done in Quick Sort. Test your program by sorting some small arrays $( n \leq 1 0 0 )$ . 

(b) Speed Test: Remove the bar and pause statement in both functions and measure the time each function needs to sort an array of 100,000 elements. Use for this the Matlab-functions tic and toc. 

(c) For fun (not efficient!): program the selection sort recursively. Use a global array and proceed similarly as with quicksort. 

3. Pythagoras Tree<sup>1</sup>: 

Basic construction: Given two points P and Q in the plane, construct the points $P ^ { \prime }$ and $Q ^ { \prime }$ to built a square. Then put on the square a right triangle with one basis angle α. 

The following figure shows the basic construction and the first recursion step, where the construction is repeated on top of the cathetes of the triangle $\overline { { P ^ { \prime } R Q ^ { \prime } } }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/61426f3bb93e98a22768eeb0ed89f44cf3e3c39cfee3f6e8140871ba54c75ae4.jpg)



Write a recursive function which computes the Pythagoras tree until the base line $\overline { { P Q } }$ becomes small. Experiment with the basis angle, choose e.g. as here in the figure $\alpha = 2 0 ^ { \circ }$


# Chapter 8 Iteration and Nonlinear Equations

## 8.1 Bisection

Consider the following problem: We are given the area $F = 1 2$ of a right-angled triangle and the section $p = 2$ of the hypotenuse (see Fig. 8.1). Compute the edges of the triangle. 

Denote with q the second section of the hypotenuse so that $c = p + q$ . The height theorem says $h _ { c } ^ { 2 } = p q$ . Replacing c and $h _ { c }$ in the expression for the area $\begin{array} { r } { F = \frac { 1 } { 2 } c h _ { c } } \end{array}$ we get 

$$
F = \frac {p + q}{2} \sqrt {p q}
$$

which is an interesting relation since it says that the area of the triangle is equal to the product of the arithmetic and the geometric mean of the two sections of the hypotenuse. Inserting the numerical values we get an equation for $x = q \mathrm { : }$ 

$$
f (x) = \frac {2 + x}{2} \sqrt {2 x} - 1 2 = 0.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/49364207df10c10b8f08b8b8c8447b6e6ad72944e26387d3c3154796ab460f5f.jpg)



Fig. 8.1 Triangle problem


We wish to find a value x such that $f ( x ) = 0$ . It is easy to see that $f ( 0 ) = - 1 2$ and $f ( 8 ) = 8$ , so we conclude, sincef is a continuous function in (0, 8), that there exists a zero in this interval. 

It is obvious to try the mid-point of the interval $\textstyle x = { \frac { 0 + 8 } { 2 } } = 4$ . We obtain $f ( 4 ) =$ $3 { \sqrt { 8 } } - 1 2 = - 3 . 5 1 4 7$ and conclude that our solution must be in the smaller interval (4, 8). Another bisection $\textstyle x = { \frac { 4 + 8 } { 2 } } = 6$ gives $f ( 6 ) = 1 . 8 5 6 4$ thus the solution must be in the interval (4, 6). We can continue this process called bisection until the two bounds are close enough to give us the solution to the precision we wish to have. 

The following function Bisekt can be used for this: 

```matlab
function x=Bisekt(f,a,b)
x=(a+b)/2;
while b-a>1e-5
    if f(x)<0,
    a=x;
    else
    b=x;
    end
    x=(a+b)/2
end 
```

Indeed we get the solution with 

```txt
>> x=Bisekt(@(x)(2+x)/2*sqrt(2*x)-12,4,6)
x =
5.3423 
```

Note that the function Bisekt must be improved to serve as a more general rootfinder. We will do that in Problem 1. 

## 8.2 Newton’s Method

Let s be a simple zero of the functionf. We want to compute s by approximatingf by a simpler function $h ( x )$ near s. The solution $x _ { 1 }$ of $h ( x ) = 0$ is then an approximation of s. Newton’s method approximatesf by the Taylor-polynomial of degree one at $x _ { 0 }$ in the neighborhood of s 

$$
h (x) = f (x _ {0}) + f ^ {\prime} (x _ {0}) (x - x _ {0}).
$$

The solution of $h ( x ) = 0$ is 

$$
x _ {1} = x _ {0} - \frac {f (x _ {0})}{f ^ {\prime} (x _ {0})}.
$$

This is called a Newton iteration step. Repeating the computation generates a sequence $\{ x _ { k } \}$ which usually converges to the solution s. 

## 8.2.1 Algorithm ofHeron

As example consider the function $f ( x ) = x ^ { 2 } - a .$ , where $a > 0$ . The positive solution of $\mathbf { \dot { \omega } } \ f ( x ) = 0 { \mathrm { i s } } s = { \sqrt { a } } .$ . Applying Newton’s method we get the iteration 

$$
x _ {k + 1} = x _ {k} - \frac {f (x _ {k})}{f ^ {\prime} (x _ {k})} = x _ {k} - \frac {x _ {k} ^ {2} - a}{2 x _ {k}} = \frac {1}{2} \left(x _ {k} + \frac {a}{x _ {k}}\right).
$$

The sequence generated by this iteration is a method to compute the square-root using only the four basic operations. It is known as the Algorithm ofHeron. In Problem 7 a careful implementation is discussed. 

## 8.2.2 Fractal

Consider the function $f ( z ) = z ^ { 3 } - 1$ . It has the three roots, one is real the other two are complex: 

$$
z _ {1} = 1, \quad z _ {2} = - \frac {1}{2} + \frac {\sqrt {3}}{2} i, \quad z _ {3} = - \frac {1}{2} - \frac {\sqrt {3}}{2} i.
$$

Using Newton’s iteration 

$$
z _ {k + 1} = z _ {k} - \frac {z _ {k} ^ {3} - 1}{3 z _ {k} ^ {2}}
$$

and complex arithmetic, the sequence $\{ \boldsymbol { z } _ { k } \}$ will converge to one ofthe roots depending of the starting value $z _ { 0 }$ . It is interesting to determine which starting point leads to which root. The set of initial values that lead to convergence to the same root is called the basin of attraction of that root. As we will see the basins of attraction of the roots have a very complicated structure, and similarly for their boundaries: they arefractal. 

We consider the region in the complex plane $\{ z = x + i y \mid - 1 \leq x , y \leq 1 \}$ . We will choose 1,000 points in each direction as starting values for Newton’s iteration. Thus a million points will be used. In the following program script we make use oftwo features of Matlab: vector-operations and meshgrid. The points are generated with the function meshgrid and stored as complex numbers in the matrix Z. The iteration is performed in parallel with the whole matrix Z. 

```matlab
clf,clc,clear
n=1000; m=30;
x=-1:2/n:1;
[X,Y]=meshgrid(x,x);
Z=X+1i*Y; % define grid for picture
for i=1:m % perform m iterations in parallel
    Z=Z-(Z.^3-1)./(3*Z.^2); % for all million points
end; % if converged then 
```

```matlab
% each element of Z contains one root
a=20; % transform roots to pos. integer values
image((round(imag(Z))+2)*a); % multiply by a to get nice colors 
```

After $m = 3 0$ iterations each element of the matrix Z has converged to one of the roots. To interpret Z as an image, we need to transform the elements to real numbers. We can distinguish the three different elements by looking at their imaginary part which is $\textstyle 0 , { \frac { \sqrt { 3 } } { 2 } } , \operatorname { o r } - { \frac { \sqrt { 3 } } { 2 } }$ . By rounding and adding 2 we get the numbers 2, 3, and 1. Now to choose nice colors we multiply them by a factor a. For a 20 we obtain the picture 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/6430ef9ede0df4fe249ebbceb5707f2b6693438616749f963d815e64ac7335ca.jpg)


## 8.3 Circular Billiard

We consider a circular billiard table and two balls located at the points P and Q, see Fig. 8.2. In which direction must the ball at point P be hit, if it is to bounce off the boundary of the table exactly once and then hit the other ball located at $Q \mathrm { ? }$ 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/0e89fcb086701c6408512b43aa671037f835699e742f65d234ea71a8052a1278.jpg)



Fig. 8.2 Billiard table


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/45e384417001ee45751b4104f48d47667d363b957ff3715acb61969782aeb7cd.jpg)



Fig. 8.3 Billiard problem


The problem does not depend on the size of the circle. Therefore, without loss of generality, we may assume the radius of the table to be 1, i.e., we will consider the unit circle. Also, the problem remains the same if we rotate the table. Thus, we may assume that one ball $( \mathrm { e . g . } Q )$ is located on the x-axis. 

The problem can now be stated as follows: In the unit circle, two arbitrary points $P = ( p _ { x } , p _ { y } )$ and $Q = ( a , 0 )$ are given. We are looking for a reflection point $X =$ (cos x, sin x) (see Fig. 8.3) on the circumference of the circle, such that a billiard ball traveling from P to X will hit Q after it bounces off the edge. The problem is solved if we know the point X, which means that we are looking for the angle x. 

The condition that must be satisfied is that the two reflection angles are equal, i.e., $\alpha _ { 1 } = \alpha _ { 2 }$ in Fig. 8.3. This is the case if the point X is the bisector of the angle $Q X P$ Thus if, $e _ { X Q }$ is the unit vector in the direction XQ, and if $e _ { X P }$ is defined similarly, then the direction of the bisector is given by the sum $\pmb { e } _ { X Q } + \pmb { e } _ { X P }$ . This vector must be orthogonal to the direction vector of the tangent $g _ { \colon }$ , 

$$
\boldsymbol {r} = \binom{\sin x}{- \cos x}.
$$

Therefore we obtain for the angle x the equation 

$$
f (x) = (\pmb {e} _ {X Q} + \pmb {e} _ {X P}) ^ {\top} \pmb {r} = 0.\tag{8.1}
$$

Let us program now the functionf(x) which we will call billiard(x). 

```matlab
function y=billiard(x)
% computes the billiard function f
global px py a
c=cos(x); s=sin(x);
X=[c;s]; P=[px;py];
XP=P-X; Ep=XP/norm(XP); % unit vector direction XP
XQ=[a-c; -s]; Eq=XQ/norm(XQ); % unit vector direction XQ
r=[s;-c]; % tangent direction vector
y=(Ep+Eq)'*r; 
```

As an example we plot the function for the following ball positions 

$P = (0.6, 0.3), Q = (-0.2, 0)$ % PlotBilliardFct.m  
clear, clc, clf  
global px py a  
px=0.6, py=0.3, a=-0.2  
F=[];  
X=0:0.01:2*pi;  
for x=X  
    F=[F, billiard(x)];  
end  
plot(X,F,[0,2*pi],[0,0]) 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/27385b42a74afc96048aa6e0578ec8ec0423c597071e1ded268dd98da892f5cc.jpg)


From this plot we see that there are two solutions for angles: one in the interval (0, 1) and the other one in (4, 5). Using bisection we get 

## 8.3 Circular Billiard

```matlab
>> [x1,y]=Bisection(@billiard,0,1)
x =
    0.504063160498908
y =
    2.220446049250313e-16
>> [x2,y]=Bisection(@billiard,4,5)
x =
    4.050212021055064
y =
    -2.220446049250313e-16 
```

## the reflection points

```matlab
format short  
>> X1=[cos(x1),sin(x1)] % first Reflection point  
X1 = 0.8756 0.4830  
>> X2=[cos(x2),sin(x2)] % second Reflection point  
X2 = -0.6148 -0.7887 
```

## Now we would like to plot the trajectories:

```matlab
% BilliardExample2.m
clf
axis equal, hold
t=0:0.01:2*pi;    % plot circle
plot(cos(t),sin(t))
plot(px,py,'o')    % plot point P
text(px,py,'    P')
plot(a,0,'o')    % plot point Q
text(a,0,'    Q')
P=[px,py]; Q=[a,0];
plot(X1(1),X1(2),'o')
text(X1(1),X1(2),'    X_1')
plot([Q(1),X1(1)], [Q(2),X1(2)])    % plot trajectory
plot([X1(1),P(1)], [X1(2),P(2)])
plot(X2(1),X2(2),'o')
text(X2(1),X2(2),'    X_2')
plot([Q(1),X2(1)], [Q(2),X2(2)])    % plot trajectory
plot([X2(1),P(1)], [X2(2),P(2)]) 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/9a09e9234a323fed21bda26f80c230c0142ff5d3fb4fd4278409ced699852086.jpg)


## 8.4 MATLAB-Elements Used in This Chapter

meshgrid: Rectangular grid in 2-D and 3-D space 

[X,Y] = meshgrid(xgv,ygv) replicates the grid vectors xgv and ygv to produce a full grid. This grid is represented by the output coordinate arrays X and Y. The output coordinate arrays X and Y contain copies of the grid vectors xgv and ygv respectively. The sizes of the output arrays are determined by the length of the grid vectors. For grid vectors xgv and ygv of length M and N respectively, X and Y will have N rows and M columns. 

imag: Imaginary part of complex number 

imag(z) returns the imaginary part of z. 

imag(A) returns the imaginary part of each element of A. 

image: Display image object 

image creates an image graphics object by interpreting each element in a matrix as an index into the figure’s colormap or directly as RGB values, depending on the data specified. 

text: Create text object in current axes 

text is the low-level function for creating text graphics objects. Use text to place character strings at specified locations. 

text(x,y,‘string’) adds the string in quotes to the location specified by the point (x,y) x and y must be numbers of class double. 

## 8.5 Problems

1. Bisection-Algorithm. Improve the function Bisekt. Your function $[ \mathbf { x } , \mathbf { y } ] =$ Bisection(f,a,b,tol) should also compute a zero for functions with $f ( a ) > 0$ andf(b) < 0 to a given tolerance tol. Be careful to stop the iteration in case the user asks for a too small tolerance! If by the bisection process we arrive at an interval $( a , b )$ which does not contain a machine number anymore then it is high time to stop the iteration. 

2. Solve with bisection the equations 

$$
(a) x ^ {x} = 5 0 (b) \ln (x) = \cos (x) (c) x + e ^ {x} = 0.
$$

Hint: a starting interval is easy to find by sketching the functions involved. 

3. Find x such that 

$$
\int_ {0} ^ {x} e ^ {- t ^ {2}} d t = 0. 5.
$$

Hint: the integral cannot be evaluated analytically, so expand it in a series and integrate. Write a function $\boldsymbol { \mathrm { \Sigma } } ( \boldsymbol { \mathrm { x } } )$ to evaluate the series. Then use bisection to compute the solution of $\ P ( x ) - 0 . 5 = 0$ 

4. Use bisection to create the following table: 

<table><tr><td>F</td><td>0</td><td><eq>0.1\pi</eq></td><td><eq>0.2\pi</eq></td><td>...</td><td><eq>\pi</eq></td></tr><tr><td>h</td><td>0</td><td>?</td><td>?</td><td>...</td><td>2</td></tr></table>

where the function $F ( h )$ is given by 

$$
F (h) = \pi - 2 \arccos \frac {h}{2} + h \sqrt {1 - \left(\frac {h}{2}\right) ^ {2}}.
$$

5. Binary search: we are given an ordered sequence of numbers: 

$$
x _ {1} \leq x _ {2} \leq \dots \leq x _ {n}
$$

and a new number z. Write a program that computes an index value i such that either $x _ { i - 1 } < z \leq x _ { i }$ or $i = 1 \mathrm { o r } i = n + 1$ holds. The problem can be solved by considering the function 

$$
f (i) = x _ {i} - z
$$

and computing its “zero” by bisection. 

6. Compute x where the following maximum is attained: 

$$
\max _ {0 <   x <   \frac {\pi}{2}} \left(\frac {1}{4 \sin x} + \frac {\sin x}{2 x} - \frac {\cos x}{4 x}\right).
$$

7. Write a function $\scriptstyle \mathbf { S } = S { \mathrm { G u a r e R o o t ~ ( a ) } }$ which computes the square root using Heron’s algorithm. Think of a good starting value and a good termination criterion. 

Hint: consider the geometrical interpretation of Newton’s method and use the (theoretical) monotonicity of the sequence as termination criterion. 

Test your function and compare the results with the standard Matlab-function sqrt. Compute the relative error of both functions. 

8. We consider again Problem 3: find x such that 

$$
f (x) = \int_ {0} ^ {x} e ^ {- t ^ {2}} d t - 0. 5 = 0.
$$

Since a function evaluation is expensive (summation of the Taylor series) but the derivatives are cheap to compute, a higher order method is appropriate. Solve this equation with Newton’s method. 

9. Using Newton’s iteration, find a such that $\int _ { 0 } ^ { 1 } e ^ { a t } d t = 2 .$ 

10. Consider the billiard-problem. Let the ball $\bar { P }$ be at position $P = ( 0 . 5 , 0 . 5 )$ and let Q move in small steps (say 0.1) from 1 to 1. 

Compute for each position the solutions using bisection. Count and plot the solutions and plot also the function billiard. make a pause before moving on the the next position of Q. 

11. Modify the fractal program by replacing $f ( z ) = z ^ { 3 } - 1$ with the function 

$$
f (z) = z ^ {5} - 1.
$$

(a) Compute the 5 zeros off using the command roots. 

(b) In order two distinguish the 5 different numbers, study the imaginary parts of the 5 zeros. Invent a transformation such that the zeros are replaced by 5 different positive integer numbers. 

12. Mandelbrot set<sup>1</sup>: Consider the iteration 

$$
Z _ {k + 1} = Z _ {k} ^ {2} + C.
$$

Depending on the value of the constant $C$ the sequence $\{ Z _ { k } \}$ will either diverge to or converge. 

Let C now be in the region in the complex plane $Z = X + i Y$ with $- 2 \leq$ $X , Y \leq 2$ 

Perform 50 iterations starting always with $Z _ { 0 } = 0$ with all numbers C in that region and plot using image the resulting Mandelbrot set, which is the set of all values C for which the iterations converges to a finite limit. 

## 9.1 Event Simulation Using Random Numbers

In this section we investigate experimental—and theoretical probabilities. The experimental probability is the quotient of the number of times the event occurs divided by the total number of trials. The theoretical probability on the other hand is the number of favorable outcomes divided by the total number of possible outcomes. 

The following example can be solved analytically and by simulation. Consider the following experiment: we are tossing a coin n 10 times. Since for a fair coin the theoretical probability for head or tail is 1/2 we expect in our experiment that k 5 times head to appear. In fact by calling the function toss a few times we obtain what we expect: 

```matlab
function k=loss(n)
k=sum(rand(1,n)<=0.5);
>> k=loss(10)
k = 5
>> k=loss(10)
k = 6
>> k=loss(10)
k = 5
>> k=loss(10)
k = 4
>> k=loss(10)
k = 7
>> k=loss(10)
k = 5
>> k=loss(10)
k = 6 
```

It is interesting to repeat the experiment, say m 100 times and to make a histogram of the numbers k obtained (see Fig. 9.1). 


Fig. 9.1 Histogram


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/4c60cf67b1d026f4c48bc6386603fa7e4a93e5aace6ae47da27cf8e890b4e275.jpg)


```matlab
% khist1.m
% Flipping a coin, histogram
clear, clf
format compact
m=100
n=10
a=zeros(1,n); % array for histogram
z=0;
for p=1:m
    k=toss(n);
    if k==0 % exception because Matlab
    z=z+1; % does not allow to use a(0)
    else
    a(k)=a(k)+1; % update array a
    end
end
axis([0,n,0,max(a)+n])
hold
bar([0:n],[z,a]) 
```

Since Matlab does not a allows zero indices we treat zero as a special case. 

Let us now compute the theoretical probability. The number of ways to get k heads in n flips is given by the binomial coefficient (“n choose k”): 

$$
\binom{n}{k}.
$$

For the theoretical probability we have to divide by the total number of possible outcomes which is (n) (n) 

$$
\frac {\binom {n} {k}}{\sum_ {j = 0} ^ {n} \binom {n} {j}} = \frac {\binom {n} {k}}{2 ^ {n}}.
$$

## 9.1 Event Simulation Using Random Numbers

Notice that the sum $\begin{array} { r } { \sum _ { j = 0 } ^ { n } \binom { n } { j } = ( 1 + 1 ) ^ { n } = 2 ^ { n } . } \end{array}$ To compute this we first need the function 

```matlab
function b=binomial(n,k)
b=1;
for j=1:k
    b=b*(n+1-j)/j;
end 
```

Then the theoretical probablity is computed by the statements 

```matlab
for k=0:n
    if k==0
    z=binomial(n,k);
    else
    f(k)=binomial(n,k); % theoretical probability
    end
end
f=f/2^n;z=z/2^n; % probability
z=z*m; f=f*m; % scaled by m
plot([0:n],[z,f],'or','LineWidth',2) 
```

This function is shown using red circles in Fig. 9.1, it has a “bell shape” which is known as normal distribution. 

By increasing m, the histogram and the theoretical probability of a given number of heads becomes smoother and approaches as limit the normal distribution: 

$\frac{1}{\sqrt{2\pi}\sigma}\exp \left(-\frac{(k - \mu)^2}{2\sigma^2}\right)$ 

where $\mu = n / 2$ is the mean and the standard deviation, a measure of the breadth of the curve width. We program this normal distribution function as 

```matlab
function y=bell(x,mu,sigma)
y=1/sqrt(2*pi)/sigma*exp(-(x-mu).^2/2/sigma^2); 
```

For equal probability coin flipping we have $\sigma = \sqrt { \mu / 2 } = \sqrt { n / 4 }$ . For n 10 and m 100 we get with 

```matlab
% khist2.m
figure(2)
axis([0,n,0,max(a)+n])
hold
plot([0:n],[z,f],'or','LineWidth',2)
sigma=sqrt(n/4)
mu=n/2
x=linspace(0,n);
plot(x,bell(x,mu,sigma)*m,'LineWidth',2) 
```

Figure 9.2 which shows already a very good match between the discrete distribution and the continuous asymptotic normal distribution. 

Consider now a larger simulation with n 100 and $m = 1 0 ^ { \prime } 0 0 0$ . We get with 


Fig. 9.2 Discrete and normal distribution


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/cb1619247510385b70e83fb9d41e178cf4fc4db6e2e3a6c7494e0c7f9880cc4c.jpg)


```matlab
% khist.m
clear, clf
format compact
m=10000
n=100
a=zeros(1,n); % array for histogram
z=0;
for p=1:m
    k=loss(n);
    if k==0 % Matlab allows no a(0)
    z=z+1;
    else
    a(k)=a(k)+1; % update array a
    end
end
axis([0,n,0,max(a)+n])
hold
bar([0:n],[z,a])
sigmaT=sqrt(n/4)
meanT=n/2
x=linspace(0,n);
plot(x,bell(x,meanT,sigmaT)*m,'r','LineWidth',2)
m =
    10000
n =
    100
Current plot held
sigmaT = 5
meanT = 50 
```

We notice first from Fig. 9.3 that the histogram matches very well the normal distribution and that it is rare that k < 40 or k > 60. In fact summing up 95 % of all cases around k 50 we get 

Fig. 9.3 Khist 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/1dbb6f04468f49dd29f0e4f0bacc19649693f9418c88ee09494a32a885d098b3.jpg)


```matlab
s=a(n/2);
p=0;
while s<=m*95/100
    p=p+1;
    s=s+a(n/2-p)+a(n/2+p);
end
p
p = 10 
```

which means that only in 5 % of all cases $k$ was outside the interval (40, 60) which is the interval meanT 2 sigmaT. 

If we do not know the theoretical mean and the standard deviation then for our histogram these two quantities can be estimated by 

$$
\mu = \frac {1}{n} \sum_ {i = 1} ^ {n} a _ {i} x _ {i}, \quad \sigma = \sqrt {\frac {1}{n} \sum_ {i = 1} ^ {n} a _ {i} (x _ {i} - \mu) ^ {2}}.
$$

For our example we obtain 

```ini
meanEx = sum(a.*[1:n])/m
deviations=[1:n]-meanEx;
variance=sum(a.*deviations.^2)/m
sigmaEx=sqrt(variance)
meanEx =
49.9325
variance =
25.2867
sigmaEx =
5.0286 
```

which compares very well with the theoretical quantities. 

## 9.2 Exhaustive Search

Exhaustive search is a problem solving technique to find an optimum in some finite space by enumerating and inspecting all possible states. 

These types of algorithms are of limited use since enumerating all permutations of n objects means inspecting a matrix with n rows and n columns. The Matlabfunction perms computes all permutations of n objects. In the description of this function we find the warning: 

This function is only practical for situations where N is less than about 10 (for N=11, the output takes over 3 gigabytes). 

It would be better not to generate and store all permutations at once but produce and use each permutation sequentially. 

On the other hand, our computers have become very powerful regarding processing time and memory. So for small but nevertheless interesting problems exhaustive search can be a valuable technique. 

As an example we consider the traveling salesman problem: Given a set of cities and the distances between each pair of cities, the problem consists in finding the shortest route which starts from a city and visits each city exactly once and finally returns to the starting city. This problem is one of the so called “hard problems” in the sense that there exists no algorithm which solves the problem in polynomial time. The number of algorithms to solve this problem approximately is large and there exist a considerable literature on this topic. In the following we shall solve the problem for a small number of cities with “brute force”. 

Consider the following distance table of some cities in Switzerland: 

<table><tr><td></td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td><td>8</td><td>9</td></tr><tr><td>1 Langenthal</td><td>0</td><td>107</td><td>47</td><td>55</td><td>37</td><td>61</td><td>50</td><td>24</td><td>80</td></tr><tr><td>2 Brienz</td><td></td><td>0</td><td>77</td><td>53</td><td>117</td><td>147</td><td>115</td><td>109</td><td>83</td></tr><tr><td>3 Bern</td><td></td><td></td><td>0</td><td>112</td><td>85</td><td>97</td><td>42</td><td>73</td><td>136</td></tr><tr><td>4 Luzern</td><td></td><td></td><td></td><td>0</td><td>65</td><td>96</td><td>105</td><td>57</td><td>31</td></tr><tr><td>5 Aarau</td><td></td><td></td><td></td><td></td><td>0</td><td>53</td><td>77</td><td>14</td><td>71</td></tr><tr><td>6 Basel</td><td></td><td></td><td></td><td></td><td></td><td>0</td><td>90</td><td>46</td><td>108</td></tr><tr><td>7 Biel</td><td></td><td></td><td></td><td></td><td></td><td></td><td>0</td><td>66</td><td>129</td></tr><tr><td>8 Olten</td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td>0</td><td>78</td></tr><tr><td>9 Zug</td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td>0</td></tr></table>

The approximate distances (in km) were taken from Google Maps. We copy this distance table in a matrix and augment it to a symmetric Matrix 

<table><tr><td>0</td><td>107</td><td>47</td><td>55</td><td>37</td><td>61</td><td>50</td><td>24</td><td>80</td></tr><tr><td>107</td><td>0</td><td>77</td><td>53</td><td>117</td><td>147</td><td>115</td><td>109</td><td>83</td></tr><tr><td>47</td><td>77</td><td>0</td><td>112</td><td>85</td><td>97</td><td>42</td><td>73</td><td>136</td></tr><tr><td>55</td><td>53</td><td>112</td><td>0</td><td>65</td><td>96</td><td>105</td><td>57</td><td>31</td></tr><tr><td>37</td><td>117</td><td>85</td><td>65</td><td>0</td><td>53</td><td>77</td><td>14</td><td>71</td></tr><tr><td>61</td><td>147</td><td>97</td><td>96</td><td>53</td><td>0</td><td>90</td><td>46</td><td>108</td></tr></table>

## 9.2 Exhaustive Search

<table><tr><td>50</td><td>115</td><td>42</td><td>105</td><td>77</td><td>90</td><td>0</td><td>66</td><td>129</td></tr><tr><td>24</td><td>109</td><td>73</td><td>57</td><td>14</td><td>46</td><td>66</td><td>0</td><td>78</td></tr><tr><td>80</td><td>83</td><td>136</td><td>31</td><td>71</td><td>108</td><td>129</td><td>78</td><td>0</td></tr></table>

To solve the traveling salesman problem for this set of cities, we first choose a start city. Assume we start with number 1 (Langenthal). Then we have to generate all permutations of the cities 2–9 (Brienz–Zug) and for each permutations add up the distances from Langenthal and back again to Langenthal. One route would then be described for instance by the numbers 

$$
1 \rightarrow 4 \rightarrow 5 \rightarrow 8 \rightarrow 6 \rightarrow 9 \rightarrow 3 \rightarrow 2 \rightarrow 7 \rightarrow 1
$$

and for the costs of this route (the sum of all km) we need to add the matrix elements 

$$
A (1, 4) + A (4, 5) + A (5, 8) + A (8, 6) + A (6, 9) + A (9, 3) + A (3, 2) + A (2, 7) + A (7, 1)
$$

which sum up to 666. 

The function TravelSalesman is now not difficult to understand 

```matlab
function [solution, minimum] = TravelSalesman(A, startCity)
% Trvelsalesman solves the traveling salesman problem
% The matrix A contains the distance table of cities. startCity is
% the Number of city where the salesman starts and returns uses
% Matlab's perms

[m, n] = size(A);
if m ~ = n,
    error('distance table is wrong')
end
if startCity > n
    error('Startcity not in the list')
end
c = []; % eliminate startCity from
for k = 1:n % the list of cities
    if k ~ = startCity
    c = [c, k];
    end
end
T = perms(c); % compute table T of all permutations
[m, p] = size(T) % add startCity as first and last city
T = [ones(m, 1) * startCity T ones(m, 1) * startCity];
minimum = inf;
for k = 1:m % for all permutations
    cost = 0;
    for j = 1: p + 1 % compute the the cost
    cost = cost + A(T(k, j), T(k, j + 1));
    end
    if cost < minimum % save the minimum cost
    minimum = cost;
    solution = T(k, :); % and the route
    end
end 
```


Fig. 9.4 Traveling salesman


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/56cf885eeae69caf24d5d5c4c3f97c73cc737fde4e640c5d74c03b30f1ab3461.jpg)


The following main program calls TravelSalesman and also plots the cities as points and the solution route, see Fig. 9.4. 

```matlab
% MainSales.m
% Main program for travelling salesman
A=[0 107 47 55 37 61 50 24 80 % distance matrix
    0 0    77 53 117 147 115 109 83
    0 0    0 112 85 97 42 73 136
    0 0    0   0 65 96 105 57 31
    0 0    0   0   0 53 77 14 71
    0 0    0   0   0   0 90 46 108
    0 0    0   0   0   0   0 66 129
    0 0    0   0   0   0   0   0   0 78
    0 0    0   0   0   0   0   0   0   0];
A=A+A'; % augment to sym. Matrix
clf
axis([0,10,0,10])
axis equal
hold
X=[3.2, 4.4 % cities as points on a map
    4.5, 0.9
    1.5, 2.4
    6.1, 2.9
    4.9, 5.9
    2.4, 7.3
    0.4, 3.8
    4.0, 5.6
    7.3, 4.1];
plot(X(:,1),X(:,2),'o')
n=9
for k=1:n
    text(X(k,1),X(k,2),[' ',num2str(k)])
end
[solution,minimum]=TravelSalesman(A,1)
plot(X(solution,1),X(solution,2)) 
```

## 9.2 Exhaustive Search

```ini
>> MainSales
Current plot held
m =
40320
p =
8
solution =
1 7 3 2 4 9 5 8 6 1
minimum =
445 
```

Starting with another city, e.g. with 2 (Brienz) yields the same result 

```julia
>> [solution, minimum] = TravelSalesman(A, 2)
m =
40320
p =
8
solution =
2 4 9 5 8 6 1 7 3 2
minimum =
445 
```

which can be expected since there is exactly one optimal route. 

## 9.3 Differential Equations

We shall consider in this section ordinary differential equations (ODEs). The solution of a differential equation is afunction. Consider as example the equation 

$$
y ^ {\prime} (x) = 2 y (x).
$$

We can guess that the solution is a exponential function since for this equation the derivative is a multiple of the function itself: 

$$
y (x) = e ^ {2 x} \quad \Longrightarrow \quad y ^ {\prime} (x) = 2 e ^ {2 x} = 2 y (x).
$$

But also $z ( x ) = a y ( x )$ with some arbitrary constant a is a solution. The equation has many solutions. To pick a specific solution we need to prescribe initial conditions. So if we consider the problem 

$$
y ^ {\prime} (x) = 2 y (x), \quad y (0) = 3
$$

then the only solution is $y ( x ) = 3 e ^ { 2 x }$ 

Differential equations have often solutions which cannot be represented by algebraic expressions. It is therefore necessary to consider numerical methods which compute approximations of the solutions. 

A curve in the plane is best described inparametricform. For instance we describe an ellipse with semi-axes a and b by 

$$
x (t) = a \cos (t), \quad y (t) = b \sin (t), \quad 0 \leq t \leq 2 \pi .
$$

When we look for a curve in the plane, the differential equation is a system oftwo equations for the functions $x ( t )$ and $y ( t )$ 

The following system of differential equations with the initial conditions $x ( 0 ) = 2$ and $y ( 0 ) = 0$ has as solution an ellipse 

$$
\begin{array}{l} {x ^ {\prime} (t) = - 2 y (t)} \\ {y ^ {\prime} (t) = \frac {x (t)}{2}.} \end{array}
$$

We can verify this with the ansatz $x ( t ) = a \cos ( t )$ and $y ( t ) = b \sin ( t )$ . It follows 

$$
\begin{array}{l} x ^ {\prime} = - a \sin t = - 2 b \sin t \implies a = 2 b \\ y ^ {\prime} = b \cos t = \frac {1}{2} a \cos t \implies b = \frac {1}{2} a. \end{array}
$$

Using the initial condition $x ( 0 ) = 2 \mathrm { w e } \operatorname* { g e t } a = 2$ and therefore $b = 1$ . So the solution of the system is the ellipse 

$$
\begin{array}{l} x (t) = 2 \cos (t) \\ y (t) = \sin (t). \end{array}
$$

## 9.3.1 Numerical Integrator ode45

Matlab provides many numerical integrators adapted for different types of ODEs (see doc ode45). A classic one if them is ode45 an implementation of the explicit Runge–Kutta (4,5) pair of Dormand and Prince. It integrates the ODE with automatic step-size control that is it adapts the step-size such that the truncation error is kept constant. 

In order to use a numerical integrator, the differential equation must be formulated in standard form as afirst order system ofdifferential equations 

$$
\mathbf {y} ^ {\prime} = \mathbf {f} (t, \mathbf {y}), \quad \text { with   initial   condition } \quad \mathbf {y} (t _ {0}) = \mathbf {y} _ {0}.
$$

Example: 

$$
y ^ {\prime \prime \prime} + 5 t y ^ {\prime \prime} + y = e ^ {- t}, \quad y (0) = 1 0, y ^ {\prime} (0) = 0, y ^ {\prime \prime} (0) = - 0. 1.
$$

This third order differential equation is transformed to a first order system by introducing new variables $z _ { 1 } ( t ) = y ( t ) , z _ { 2 } ( t ) = y ^ { \prime } ( t )$ and $z _ { 3 } ( t ) = y ^ { \prime \prime } ( t )$ . Then by differentiating and replacing the y we get the system 

$z_1' = y' = z_2$ $z_2' = y'' = z_3$ $z_3' = y''' = -5ty'' - y + e^{-t} = -5tz_3 - z_1 + e^{-t}$ 

which written in matrix-vector notation is 

$$
\boldsymbol {z} ^ {\prime} = A \boldsymbol {z} + \boldsymbol {b} \quad A = \left( \begin{array}{c c c} 0 & 1 & 0 \\ 0 & 0 & 1 \\ - 1 & 0 & - 5 t \end{array} \right), \boldsymbol {b} = \left( \begin{array}{c} 0 \\ 0 \\ e ^ {- t} \end{array} \right).
$$

The initial conditions for this system are $z ( 0 ) = [ 1 0 , 0 , - 0 . 1 ] ^ { \top }$ 

The Matlab function ode45 can be used to solve such a first order system of ODEs. We need to define the system as a function odefun. For a scalar t and a vector y, odefun $( \operatorname { t } , \operatorname { y } )$ must return a column vector corresponding to $f ( t , y )$ Then the ODE is integrated with 

```txt
[tout,yout] = ode45(odefun,tspan,y0) 
```

where tspan indicates the interval for which the functions should be computed, so for instance we could have tspan=[0,10]. The third parameter $\mathtt { y 0 }$ contains the values of the initial conditions. The output parameters are [tout,yout]. Each row in the solution array yout corresponds to the function values $z _ { 1 } , \ldots , z _ { n }$ at a time returned in the column vector tout. 

For our example we first program the function 

```matlab
function dz=fsystem(t,z)
A=[0 1 0
    0 0 1
    -1 0 -5*t];
b=[0 0 exp(-t)]';
dz=A*z+b; 
```

The main program is then 

```matlab
% Example for ode45
t=0; y0=[10 0 -0.1]';
[tt,yy]=ode45(@fsystem,[0,5],y0)
plot(tt,yy) 
```

It produces a table of results and a plot of the functions $z _ { 1 } ( t ) = y ( t )$ (blue color), $z _ { 2 } ( t ) = y ^ { \prime } ( t )$ (green color) and $z _ { 3 } ( t ) = y ^ { \prime \prime } ( t )$ (red color), see Fig. 9.5. 


Fig. 9.5 Third order ODE


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/d2b7a99bea16a8168748f06c0d3bbd9bc0352fb6579b732d671f650de34d688f.jpg)


## 9.3.2 Dog Attacking a Jogger

This example is taken from [4]. We consider the following problem: while a jogger is running on some trail in the plane, he is being attacked by a dog. Compute the orbit $x ( t ) , y ( t )$ of the dog. 

We assume that the dog is running full speed with constant velocity w. His velocity vector points at every time to its goal, the jogger. We assume that the motion of the jogger is described by the two functions $X ( t )$ and $Y ( t )$ . The following equations hold: 

1. $\dot { x } ^ { 2 } + \dot { y } ^ { 2 } = w ^ { 2 }$ : The dog is running with constant speed. 

2. The velocity vector of the dog is parallel to the difference vector between the position of the jogger and the dog: 

$$
\binom{\dot {x}}{\dot {y}} = \lambda \binom{X - x}{Y - y} \text { with } \lambda > 0.
$$

If we substitute this in the first equation we obtain 

$$
w ^ {2} = \dot {x} ^ {2} + \dot {y} ^ {2} = \lambda^ {2} \left| \left| \binom{X - x}{Y - y} \right| \right| ^ {2}.
$$

This equation can be solved for λ: 

$$
\lambda = \frac {w}{\left| \left| \binom {X - x} {Y - y} \right| \right|} > 0.
$$

Finally, substitution of this expression for λ in the second equation yields the differential equation of the orbit of the dog: 

$$
\binom{\dot {x}}{\dot {y}} = \frac {w}{\left| \left| \binom{X - x}{Y - y} \right| \right|} \binom{X - x}{Y - y}.\tag{9.1}
$$

To solve this system we need to program several functions. First the trail of the jogger. We let him run on the x-axis: 

```javascript
function s=jogger1(t);
s=[8*t; 0]; 
```

Next we program the ODE for the dog: 

```matlab
function dz=dog1(t,z)
global w
X=jogger1(t);
h=X-z;
nh=norm(h);
dz=w/nh*h; 
```

The main program then becomes 

```matlab
% mainDog1
global w
y0=[60;70]; % starting point of the dog
w=10; % w speed of the dog
[t,Y]=ode45(@dog1,[0,10],y0)
clf; hold on;
axis([-10,100,-10,70]);
plot(Y(:,1),Y(:,2));
J=[]; % recompute the trail of the
for k=1:length(t), % jogger for the same points
    w=jogger1(t(k)); % in time as used for the dog
    J=[J; w'];
end;
plot(J(:,1), J(:,2),'r'); 
```

To plot the trail of the jogger we recompute it using the same points in time as were used for the dog’s orbit. This will be also useful for showing the movements (see below). We get the following result, see Fig. 9.6. Since the dog is running faster (with speed 10) than the jogger (with speed 8), by integrating a little longer the dog should catch the jogger. However, the system (9.1) has a singularity when the dog reaches the jogger: the norm of the difference vector becomes zero and we should stop the integration, since also the numerical integrator gets in trouble. 

We do not know the exact time when this happens, so we should stop integrating when the dog is near the jogger. For such situations Matlab provides the possibility to define another termination criterion for the integration, different from a given upper bound for the independent variable. It is possible to terminate the integration by checking zero crossings of a function. 


Fig. 9.6 Dog orbit (blue), jogger trail (red)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/b1e8d905a21d50f80c498a65226912ae42c3091c53acf2e816c968529cad52ef.jpg)


To do so we need to add in the main programm a call to the function odesets 

```python
options= odeset('events', 'on') 
```

to trigger Matlab to observe events. The paramenter options has to be passed to ode45 as additional input parameter: 

```javascript
[t,Y]=ode45('dog2',[0,30],y0,options) 
```

Furthermore the function describing the dog’s movement has to be adapted, we would like to terminate integration when $\left| \left| ( \bar { X } - x , Y - y ) ^ { \top } \right| \right|$ becomes small. In order to do so we have to add a third input and two more output parameters to the function describing the dog. 

```matlab
function [dz,isterminal,direction]=dog2(t,z,flag);
% 
global w    % w = speed of the dog
X=jogger1(t);
h=X-z;
nh=norm(h);
if nargin<3|isempty(flag) % normal output
    dz=(w/nh)*h;
else 
    switch(flag)
    case 'events'    % at norm(h)=0 there is a singularity
    dz= nh-1e-3;    % zero crossing at pos_dog=pos_jogger
    isterminal= 1;    % this is a stopping event
    direction= 0;    % don't care if decrease or increase
    otherwise 
    error(['Unknown flag: ' flag]);
    end 
end 
```

The integrator ode45 calls the function in two ways: The first one consists of dropping the third parameter. The function then returns only the parameter dz: the speed of the dog. In the second way the keyword ’events’ is assigned to the parameter flag. This keyword tells the function to return the zero-crossing function in the first output dz. The second output isterminal is a logical vector that tells the integrator, which components of the first output force the procedure to stop when they become zero. Every component with this property is marked with a nonzero entry in isterminal. The third output parameter direction is also a vector that indicates for each component of dz if zero crossings shall only be regarded for increasing values (direction = 1), decreasing values (direction = -1) or in both cases (direction = 0). The condition for zero crossings is checked in the integrator. The main program becomes 

```matlab
% mainDog2
global w
y0=[60;70];    % starting point of the dog
w=10;    % w speed of the dog
options=odeset('Events','on')
[t,Y]=ode45('dog2',[0,10],y0,options)
clf; hold on;
axis([-10,120,-10,80]);
plot(Y(:,1),Y(:,2));
J=[];
for k=1:length(t),
    w=jogger1(t(k));
    J=[J; w'];
end;
plot(J(:,1), J(:,2),'*r'); 
```

and we get the Fig. 9.7. 

I would be nice to show the movement dynamically. For this we plot for each time interval piecewise the orbit of the dog and the trail of the jogger. In order to not delay the plotting we have to include the command drawnow in the loop. We also include a pause-statement to slow down the computation, so that the movements become nicely visible. Thus the program becomes 


Fig. 9.7 Integrating till dog reaches the jogger


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/10ab9c80d0e41b6477092fbc40de5e62e8e2d20c9e55394fd798faadcc5d2678.jpg)


```matlab
% mainDog3
global w
y0=[60;70];    % starting point of the dog
w=10;    % w speed of the dog
options=odeset('Events','on')
[t,Y]=ode45('dog2',[0,10],y0,options)
clf; hold on;
axis([-10,120,-10,80]);
J=[];
for k=1:length(t),
    w=jogger1(t(k));
    J=[J; w'];
end;
title ('Dog Attacking Jogger');
for h=1:length(t)-1,
    plot ([Y(h,1),Y(h+1,1)],[Y(h,2),Y(h+1,2)]);
    plot ([J(h,1),J(h+1,1)],[J(h,2),J(h+1,2)],'r')
    drawnow;
    pause(0.05);
end
hold off; 
```

## 9.4 MATLAB-Elements Used in This Chapter

## sum: Sum of array elements

If A is a vector, then sum(A) returns the sum of the elements. If A is a matrix, then sum(A) returns a row vector containing the sum of each column. 

## perms: All possible permutation

P = perms(v) returns a matrix containing all permutations of the elements of vector v in reverse lexicographic order. Each row of P contains a different permutation of the n elements in v. Matrix P has the same data type as v, and it has n! rows and n columns. 

## ode45: Solve nonstiff differential equations; medium order method

odefun: A function handle that evaluates the right side of the differential equations y’ = f(t,y) 

tspan: A vector specifying the interval of integration, [t0,tf]. ode45 imposes the initial conditions at tspan(1), and integrates from tspan(1) to tspan(end). To obtain solutions at specific times (all increasing or all decreasing), use tspan = [t0,t1,…,tf]. 

options: Structure of optional parameters that change the default integration properties. This is the fourth input argument. 

You can create options using the odeset function. See odeset for details. 

odeset: Create or alter options structure for ordinary differential equation solvers 

options = odeset(’name1’,value1,’name2’,value2,…) creates an options structure that you can pass as an argument to the ode45 solver. In the resulting structure, options, the named properties have the specified values. For example, ’name1’ has the value value1. Any unspecified properties have default values. It is sufficient to type only the leading characters that uniquely identify a property name. Case is ignored for property names. 

## 9.5 Problems

1. Waiting for the elevator. We consider a building with n floors. A elevator is serving these floors and we are interested to know the distribution of the waiting time from pressing the elevator button till the elevator opens the door. 

Assume the time unit for the moving of the elevator one floor is one. We make m experiments in which the elevator is randomly located on one floor and the person is also coming randomly on one floor. The difference of the two floors is proportional to the time the elevator needs to come. 

Perform $m = 1 0 ^ { \prime } 0 0 0$ experiments for a $. n = 5 0$ floors building. Construct and plot the histogram of the waiting times. 

2. Given a set of points in the unit square. Write a program which computes and plots the two closest points. 

(a) Writeafunction [P,Q,minimum]=ClosestPoints $( \mathbf { x } , \mathbf { y } )$ which computes all the distances between two points and stores the minimal distance and the two points P and Q which are closest. 

(b) Generate n points $( x _ { k } , y _ { k } )$ using the function rand. Then call the function ClosestPoints, plot the points and mark the two closest points by coloring them differently. 

3. Shortest distance between two point sets: 

(a) Consider the circle with center (5, 6) and radius $r = 2$ and the ellipse with center at origin and $a = 1$ and $b = 0 . 5$ parallel to the coordinate axis. Sample points on the ellipse and on the circle. Compute by brute force a point P on the circle and a point Q on the ellipse with minimal distance. 

(b) The circle with center (5, 6) and radius $r = 2$ and the ellipse with center $( 4 , 4 )$ , $a = 2$ and $b = 3$ intersect. Try to compute the intersection points by brute force. 

4. Knapsack Problem: given a bag with a given maximum load limit W. Put in that bag items from the following table in order to maximize the sum of the value of the items but not exceeding the total weight W: 

<table><tr><td>item</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td></tr><tr><td>weights</td><td>3.3</td><td>4.6</td><td>1.7</td><td>5.8</td><td>7.7</td><td>3.1</td><td>5.3</td></tr><tr><td>values</td><td>7</td><td>9</td><td>5</td><td>12</td><td>14</td><td>6</td><td>12</td></tr></table>

Write a brute force program that solves the problem for a collections of bags: 

$$
\mathrm{W} = [ 8, 1 0, 1 1, 1 5, 2 0, 2 1, 2 5, 2 6, 3 0, 3 2 ]
$$

5. A dog would like to cross a river of width b. He starts at point $( b , 0 )$ with the goal to swim to (0, 0) where he has detected a sausage. His swim velocity $v _ { D }$ is constant and his nose points always to the sausage. The river flows north in direction of the y-axis and velocity of the flow of the river $v _ { R }$ is everywhere constant. 

(a) Develop the differential equation describing the orbit ${ \boldsymbol { z } } ( t ) = ( x ( t ) , y ( t ) ) ^ { \top }$ of the dog. 

(b) Program a Matlab function $\scriptstyle \mathtt { z p = d o g ( t , z ) }$ which describes the differential equation. The velocities $v _ { D }$ and $v _ { R }$ may be declared as global variables. 

(c) Use the program quiver and plot the slope field for $b = 1 , v _ { R } = 1$ and the following three cases for the dog velocity $v _ { D } = 0 . 8 , 1 . 0$ and 1.5. 

Note: quiver $( \mathrm { { X } } , \mathrm { { Y } } , \mathrm { { X p } } , \mathrm { { Y p } ) }$ needs 4 matrices. X and Y contain the coordinates of the points and Xp and Yp the two components of the velocity at that point. To compute these you can use the function dog e.g. 

$$
z = \operatorname{dog} (0, [ X (k, j), Y (k, j) ]); X p (k, j) = z (1); Y p (k, j) = z (2);
$$

(d) Develop a Matlab integrator for the method of Heun of order 2 

```matlab
function Z= OdeHeun(f,z0,tend,n)
% ODEHEUN integrates y'=f(t,y), y(0)=z0 with Heun
% from t=0 to tend using a fixed step size h=tend/n 
```

which integrates a given system of differential equations $\mathbf { y } ^ { \prime } = f ( t , \mathbf { y } )$ and stores the results in the matrix Z.The i th row of the matrix Z contains the values 

$$
[ t _ {i}, y _ {1} (t _ {i}), \dots , y _ {n} (t _ {i}) ].
$$

Compute and plot the orbits for the three dog velocities. You may want to stop the integration before executing all n steps when the dog arrives close to the origin or in the case when $v _ { D } < v _ { R }$ the dog is near the y-axis. 

Hint: An approximation $y _ { k } \approx y ( t _ { k } )$ ofthe solution ofthe differential equation $y ^ { \prime } = f ( t , y ) , y ( t _ { 0 } ) = y _ { 0 }$ is computed for constant stepsize h by the method of Heun with the following statements 

$$
k = 0, 1, 2, \ldots
$$

$$
k _ {1} = f (t _ {k}, y _ {k})
$$

$$
y ^ {*} = y _ {k} + h k _ {1}
$$

$$
k _ {2} = f (t _ {k} + h, y ^ {*})
$$

$$
y _ {k + 1} = y _ {k} + \frac {h}{2} (k _ {1} + k _ {2})
$$

$$
t _ {k + 1} = t _ {k} + h
$$

## 10.1 Chapter 1: Starting

1. Start Matlab with the GUI and watch the introductory video and study the tutorial. 

2. If you own a computer or laptop without Matlab then download and install the open source software GNU Octave on it. 

## 10.2 Chapter 2: How a Computer Calculates

1. Consider the following finite decimal arithmetic: 2 digits for the mantissa and one digit for the exponent. So the machine numbers have the form $\pm Z . Z \mathrm { E } \pm Z$ where $Z \in \{ 0 , 1 , \ldots , 9 \}$ 

(a) How many normalized machine numbers are available? 

(b) Which is the overflow- and the underflow range? 

(c) What is the machine precision? 

(d) What is the smallest and the largest distance of two consecutive machine numbers? 

Solution: 

We first count the machine numbers. We can form 19 different exponents: $- 9 , - 8 , \ldots , 9$ . The first digit, before the decimal point, can not be zero, because we consider only normalized numbers, thus we have 9 possibilities for the first digit. Thus in total we have $2 \times 9 \times 1 0 \times 1 9 = 3 4 2 0$ normalized machine numbers plus the number zero. Therefore the grand total is 3421 machine numbers. 

The largest number is $9 . 9 \mathrm { E } 9 = 9 , 9 0 0 , 0 0 0 , 0 0 0$ and the smallest positive number is 1.0E 9. The overflow range is $| x | > 9 . 9 \mathrm { E } 9$ and the underflow range is $0 < | x | < 1 . 0 \mathrm { E } { - 9 }$ 

The machine precision is the spacing between the numbers in (1, 2) thus $\varepsilon = 1 . 1 \mathrm { E } 0 - 1 . 0 \mathrm { E } 0 = 1 \mathrm { E } - 1 .$ 

The largest distance between two machine numbers occurs when the exponent is $9 ; 9 . 9 \mathrm { E } 9 - 9 . 8 \mathrm { E } 9 = 1 \mathrm { E } 8$ . The smallest distance is $1 . 1 \mathrm { E } { - } 9 - 1 . 0 \mathrm { E } { - } 9 =$ 1E 10. 

## 2. Solving a quadratic equation: Write a Matlab function

```txt
function [x1, x2] = QuadraticEq(p, q) 
```

which computes the real solutions of an equation 

$$
x ^ {2} + p x + q = 0.
$$

If the solutions turn out to be complex then write an error message. Test your program with the following examples: 

(x 2)(x 3) x<sup>2</sup> x 6 0 thus p 1 and q 6. 

$( x - 1 0 ^ { 9 } ) ( x + 2 \cdot 1 0 ^ { - 9 } ) = x ^ { 2 } + ( 2 \cdot 1 0 ^ { - 9 } - 1 0 ^ { 9 } ) x + 2$ 

thus $p = 2 e { - } 9 - 1 e 9$ and $q = - 1 e 9 .$ 

(x 10<sup>200</sup>)(x 1) x<sup>2</sup> (10<sup>200</sup> 1)x 10<sup>200</sup> 

thus $p = 1 e 2 0 0 - 1$ and $q = - 1 e 2 0 0$ 

Comment your results. 

Solution: Using the textbook formula 

$$
x _ {1, 2} = - \frac {p}{2} \pm \sqrt {\left(\frac {p}{2}\right) ^ {2} - q}
$$

we obtain the function 

function [x1,x2]=QuadEquationNaive(p,q)
discriminant=(p/2)^2-q;
if discriminant<0
    error('solutions are complex')
end

d=sqrt(discriminant);
x1=-p/2+d; x2=-p/2-d;

We test this function:
• $(x-2)(x+3)=x^{2}+x-6=0$ >> [x1,x2]=QuadEquationNaive(1,-6)
    x1=2, x2=-3 correct
• $(x-10^{9})(x+2\cdot10^{-9})=x^{2}+(2\cdot10^{-9}-10^{9})x-2$ >> [x1,x2]=QuadEquationNaive(2e-9-1e9,-2)
    x1=1.0000e+09, x2=0 wrong 

- $(x + 10^{200})(x - 1) = x^2 + (10^{200} - 1)x - 10^{200}$ >> [x1, x2] = QuadEquationNaive(1e200 - 1, -1e200)
x1 = Inf, x2 = -Inf wrong 

Why do we get wrong answers? When looking at the textbook formula we notice that for large $| p |$ forming $p ^ { 2 }$ may overflow. This is the case in the third example. On the other hand for small q the formula is 

$$
x _ {1, 2} = - \frac {p}{2} \pm \sqrt {\left(\frac {p}{2}\right) ^ {2} - q} \approx - \frac {p}{2} \pm \frac {p}{2}
$$

and one solution is affected by cancellation. This is the case in the second example. 

We can avoid the overflow by factoring out. The cancellation can be avoided by computing first the solution which has the larger absolute value and then use the relation of Vieta: 

$$
x _ {1} x _ {2} = q
$$

to compute the smaller solution without cancellation. Thus instead of the textbook formula we use 

$$
\begin{array}{l} x _ {1} = - \text { sign } (p) \left(| p | / 2 + | p | \sqrt {\frac {1}{4} - q / p / p}\right) \\ x _ {2} = q / x _ {1} \quad \text { Vieta } \end{array}
$$

We obtain the function 

```matlab
function [x1,x2]=QuadraticEq(p,q)
if abs(p/2)>1 % avoid overflow
    factor=abs(p); discriminant=0.25-q/p/p; % by factoring out
else
    factor=1; discriminant=(p/2)^2-q;
end
if discriminant<0
    error('Solutions are complex')
else
    x1=abs(p/2)+factor*sqrt(discriminant); % compute larger solution
    if p>0, x1=-x1; end % adapt sign
    if x1== 0, x(2)=0;
    else
    x2=q/x1; % avoid cancellation
    end % for smaller solution
end 
```

This time we get 

- $(x - 2)(x + 3) = x^2 + x - 6 = 0$ >> [x1, x2] = QuadraticEq(1, -6)    x1 = 2    x2 = -3 

correct
- $(x - 10^{9})(x + 2 \cdot 10^{-9}) = x^{2} + (2 \cdot 10^{-9} - 10^{9})x - 2$ >> [x1,x2]=QuadraticEq(2e-9-1e9,-2) x1=1.0000e+09 x2=-2.0000e-09
correct!
- $(x + 10^{200})(x - 1) = x^{2} + (10^{200} - 1)x - 10^{200}$ >> [x1,x2]=QuadraticEq(1e200-1,-1e200) x1=-1.0000e+200 x2=1
correct! 

## 10.3 Chapter 3: Plotting Functions and Curves

## 1. We are given the points

```csv
x|0.9 2.3 3.9 4.6 5.8 7.3
y|2.9 4.1 4.8 7.0 7.0 8.7 
```

(a) Define a region to plot the points using axis. Use hold to freeze the axis. 

(b) Plot the points using the symbol $\cdot _ { \mathrm { x } } ,$ 

(c) We want to fit a regression line through the points, that means compute the parameters a and b such that 

$$
y _ {k} = a x _ {k} + b, \quad k = 1, \ldots , 6.
$$

This is a linear system of equations with two unknowns and 6 equations. It cannot be solved exactly, the equations contradict themselves. However, the Matlab -operator does solve the system in the least squares sense by computing the best approximation for all equations. Form the linear system $A \left( { a \atop b } \right) = { \bf y }$ and solve it by A y 

(d) Using the computed values of a and b, plot the regression line on the same plot with the points. 

## Solution:

```matlab
x=[0.9 2.3 3.9 4.6 5.8 7.3]'
y=[2.9 4.1 4.8 7.0 7.0 8.7]'

axis([0,8,0,9])
hold
plot(x,y,'x')
A=[x,ones(size(x))]
z=A\y
a=z(1); b=z(2);
plot(x,a*x+b) 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/2c04b7d93da7547d0ef39cc83c165ed55f83156a9c5a92065c7ecf92aa7381df.jpg)


## 2. Ellipse plots.

(a) Plot the ellipse with center in origin and the main axis $a = 3$ on the x-axis and minor axis $b = 1$ . Plot also the center using the symbol $\cdot _ { + } \cdot$ 

(b) Now move the ellipse so that the center is the point $( 4 , - 1 )$ and the direction of the main axis has an angle of $- 3 0 ^ { \circ }$ with the x-axis. Plot this new ellipse in the same frame. 

Hint: Use a rotation matrix of the form 

$$
Q = \left( \begin{array}{c c} \cos \alpha & - \sin \alpha \\ \sin \alpha & \cos \alpha \end{array} \right)
$$

to rotate the coordinates of the ellipse. 

## Solution:

```matlab
clear, clf
axis([-4,8,-4,8])
axis equal % both axes same units
hold
a=3, b=1
t=0:0.01:2*pi;
x=a*cos(t)
y=b*sin(t)
pause
plot(0,0,'+') % plot first ellipse with center
plot(x,y)
alpha=-pi/6 % -30 degrees % rotation angle
c=cos(alpha), s=sin(alpha)
Q=[c -s; s c] % rotation matrix
pause
E=ones(2,length(x)); 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/534a3db6c8d146fac2e7b7176ded2f8cf7e8cdbd8531c12dbbb5287ec2a72613.jpg)


3. Plot for $- 3 \leq x \leq 3$ and $- 5 \leq y \leq 5$ the function $f ( x , y ) = x ^ { 2 } - 2 y x ^ { 3 }$ using contour and mesh. 

## Solution:

```matlab
clear, clf
[x,y]=meshgrid(-3:0.1:3,-5:0.1:5);
z=x.^2-2*y.*x.^3;
figure(1)
mesh(x,y,z)
figure(2)
contour(x,y,z,250) 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/a7f78fabddd598a16b50fb9d555d2bbf1eedfd4e3ff66658412a7b448765469f.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/06bd43e0e4156c0b7a3059c683c23b82158199f80412da4e35e445e9b7e61f5f.jpg)


## 10.4 Chapter 4: Some Elementary Functions

1. Explain what happens in Algorithm e1 when x 20. 

Hint: look at the size of the largest term and at the final result. What happens when computing the result in finite arithmetic? 

Solution: For large negative x, e.g. for x 20 and x 50, we obtain using the function e1 

```txt
>> e1(-20)
ans = 5.621884807271559e-09
>> exp(-20)
ans = 2.061153622438558e-09
>> e1(-50)
ans = 1.107293448191918e+04
>> exp(-50)
ans = 1.928749847963918e-22 
```

which are completely incorrect. The reason is that for x 20, the terms in the series 

$$
1 - \frac {2 0}{1 !} + \frac {2 0 ^ {2}}{2 !} - \dots + \frac {2 0 ^ {2 0}}{2 0 !} - \frac {2 0 ^ {2 1}}{2 1 !} + \dots
$$

become large and have alternating signs. The largest terms are 

$$
\frac {2 0 ^ {1 9}}{1 9 !} = \frac {2 0 ^ {2 0}}{2 0 !} = 4. 3 e 7.
$$

The partial sums should converge to $e ^ { - 2 0 } = 2 . 0 6 e { \mathrm { - } } 9$ . But because of the growth of the terms, the partial sums become large as well and oscillate as shown in 


Fig. 10.1 Partial sums of the Taylor expansion of $e ^ { - 2 0 }$


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/f3581d0dcd9fd8f015a08895f2fe6c031f538f07e092ae906ec285f54fe7b8c2.jpg)



Table 10.1 Numerically computed partial sums of $e ^ { - 2 0 ^ { 1 } }$


<table><tr><td>Number of terms summed</td><td>Partial sum</td></tr><tr><td>20</td><td>-2.182259377927747e+07</td></tr><tr><td>40</td><td>-9.033771892137873e+03</td></tr><tr><td>60</td><td>-1.042344520180466e-04</td></tr><tr><td>80</td><td>6.138258384586164e-09</td></tr><tr><td>100</td><td>6.138259738609464e-09</td></tr><tr><td>120</td><td>6.138259738609464e-09</td></tr><tr><td>Exact value</td><td>2.061153622438558e-09</td></tr></table>

Fig. 10.1. Table 10.1 shows that the largest partial sum has about the same size as the largest term. Since the large partial sums have to be diminished by additions/subtractions ofterms, this cannot happen without cancellation. Neither does it help to first sum up all positive and negative parts separately, because when the two sums are subtracted at the end, the result would again suffer from catastrophic cancellation. Indeed, since the result 

$$
e ^ {- 2 0} \approx 1 0 ^ {- 1 7} \frac {2 0 ^ {2 0}}{2 0 !}
$$

is about 17 orders of magnitude smaller than the largest intermediate partial sum and the IEEE Standard has only about 16 decimal digits of accuracy, we cannot expect to obtain even one correct digit! To obtain a correct value to 16 digits we would have to compute with over 30 digits. 

2. Write a Matlab-function to compute sin x using the series (4.7). In order to avoid cancellation for large x reduce the argument to the interval /2, /2 . 

```txt
Solution: 
```

The reduction of the arguments x to the interval $[ - \pi / 2 , \pi / 2 ]$ is important because the series is alternating and the summation will be affected by catastrophic cancellation for large x . We first reduce the angle to 0, 2π using the mod-function and then in a second step to $[ - \pi / 2 , \pi / 2 ]$ . For very large arguments the reduction by the mod-function will be inaccurate. So we must expect then a less accurate result. 

```matlab
function s=MySin(x);
% MYSIN Machine-independent computation of sin(x)
% using Taylor Series
if x<0, v=-1; x=-x; else v=1; end % store sign
x=mod(x,2*pi); % reduce angle to [0,2*pi]
if x>pi, x=x-pi; v=-v; end % further reductions
if x>pi/2, x=pi-x; end % so that
if v==-1, x=-x; end % -pi/2<x<pi/2
s=x; t=x; i=1; sold=2*x; % sum the series
while s~=sold,
    sold=s; i=i+2;
    t=-t*x/(i-1)*x/i;
    s=sold+t;
end

>> x=1000; [MySin(x)-sin(x)]
ans =
    2.1760e-14
>> x=10; [MySin(x)-sin(x)]
ans =
    -2.2204e-16
>> x=1e10; [MySin(x)-sin(x)]
ans =
    3.4036e-07
>> x=-1000; [MySin(x)-sin(x)]
ans =
    -2.1760e-14 
```

## 3. Do the same for cos x.

Solution: We proceed similarly as with MySin. The reduction needs adjustment. 

```matlab
function s=MyCos(x)
% MYCOS Machine-independent computation of cos(x)
% using Taylor Series
x=abs(x); v=1; % cos is symmetric
x=mod(x,2*pi); % reduce angle to [0,2*pi]
if x>3*pi/2,
    x =x-2*pi; % further reductions 
```

```matlab
elseif x>pi/2, % so that
    x=x-pi; v=-1; % -pi/2<x<pi/2
end
s=1; t=1; i=0; sold=2; % sum the series
while s~=sold,
    sold=s; i=i+2;
    t=-t*x/(i-1)*x/i;
    s=sold+t;
end
if v==-1,s=-s;end % adjust sign of function
>> x=1; [MyCos(x)-cos(x)]
ans =
-1.1102e-16
>> x=10; [MyCos(x)-cos(x)]
ans =
2.2204e-16
>> x=-100; [MyCos(x)-cos(x)]
ans =
2.1094e-15
>> x=1000; [MyCos(x)-cos(x)]
ans =
-3.2196e-14
>> x=1e10; [MyCos(x)-cos(x)]
ans =
1.9004e-07 
```

4. Combine both functions and write a function to compute tan x. 

Solution: we just use the relation tan x sin x cos x 

```matlab
function y=MyTan(x)
% MYTAN compute tan(x) using only the four basic operations.
% refers to MySin and MyCos.
y=MySin(x)/MyCos(x);

>> x=1e10; [MyTan(x)-tan(x)]
ans =
5.1134e-07
>> x=300; [MyTan(x)-tan(x)]
ans =
2.3782e-11
>> x=30; [MyTan(x)-tan(x)]
ans =
5.0626e-14 
```

5. Write a function to compute arctan x for x < 1 using the series (4.8) and compare your result with the standard Matlab-function atan(x). 

```matlab
Solution:
function s=MyArctan(x)
% MYARCTAN computes the function arctan(x) 
```

## 10.4 Chapter 4: Some Elementary Functions

```matlab
% for |x|<1
s=x; t=x; k=1; sold=0;
while s~=sold
    sold=s; k=k+2; t=-t*x^2;
    s=s+t/k;
end

>> for x=[0.7,-0.7,0.5,-0.5,0.1,-0.1]
    [MyArctan(x)-atan(x)]
    end
ans =
    1.1102e-16
ans =
    -1.1102e-16
ans =
    -2.2204e-16
ans =
    2.2204e-16
ans =
    -2.7756e-17
ans =
    2.7756e-17 
```

## 10.5 Chapter 5: Computing with Multiple Precision

For the following problems, make use of the functions we developed for computing Euler’s number e. 

1. Compute using multiple precision the powers of 2: 

$2^{i},\quad i = 1,2,\ldots ,300$ 

Solution: 

```matlab
function Power2(m)
% POWER2 computes the powers of 2 in multiple precision
% 2^k, k=0, ..., m
n=round(m*log10(2))+1; % compute how many array elements we need
c=10; % we pack one digit in one element
a=zeros(1,n,'uint32');
a(n)=1;
for k=1:m
    a=a*2; % generate next power of 2
    a=Carry(c,a);
    ['2',sprintf('%01d',k), ' = ', sprintf('%01d',a)]
end 
```

2. Write a program to compute factorials using multiple precision: 

$n!, n = 1,2,\ldots,200$ 

Solution: It is not simple to predict how many decimal digits are needed to represent the number n The Scottish mathematician James Stirling derived the asymptotic formula 

$$
n! \sim \sqrt {2 \pi n} \left(\frac {n}{e}\right) ^ {n}.
$$

We can estimate using log10 the number of digits. Don’t just take the logarithm of the above expression! It will become already Inf for $n < 2 0 0$ . We have to split the expression in several logarithms 

$$
\log 1 0 (n!) = \log 1 0 (\sqrt {2 \pi n}) + n \log 1 0 (n) - n \log 1 0 (e)
$$

to avoid overflow. 

```matlab
function Factorials(n)
% FACTORIALS computes k! for k=1,...,n in multiple precision
% use Stirlings formula to estimate number of digits
m=round(log10(sqrt(2*pi*n))+n*(log10(n)-log10(exp(1))))
c=10;    % we pack one digit in one element
a=zeros(1,m,'uint32');
a(m)=1;
for k=1:n
    a=a*k;    % generate k!
    a=Carry(c,a);
    [sprintf('%01d',k), '!' = ', sprintf('%01d',a)]
end 
```

3. Compute to 1000 decimal digits. Use the relation by C. Størmer: 

$$
\pi = 2 4 \arctan {\frac {1}{8}} + 8 \arctan {\frac {1}{5 7}} + 4 \arctan {\frac {1}{2 3 9}}.
$$

## Hints:

Compute first a multiprecision arctan function using the Taylor-series (4.8) as proposed in Chap. 4: 

$$
\arctan x = \sum_ {k = 0} ^ {\infty} (- 1) ^ {k} \frac {x ^ {2 k + 1}}{2 k + 1} = x - \frac {x ^ {3}}{3} + \frac {x ^ {5}}{5} - \dots
$$

The above series is alternating so there is a danger of cancellation. However, since it is used only for $| x | < 1$ this is not much a concern. What we need is a new function Sub 

```matlab
function r=Sub(c,a,b)
% SUB computes r=a-b where a and b are multiprecision numbers
% with a>b. 
```

to subtract two multiprecision numbers. One has to be careful not to generate negative numbers, all intermediate results have to remain positive. 

To compute we have to evaluate for some integer $p > 1$ the function arctan $( 1 / p )$ . When generating the next term after 

$$
t _ {k} = \frac {x ^ {2 k + 1}}{2 k + 1}
$$

for $x = 1 / p$ we have to form 

$$
t _ {k + 1} = t _ {k} / p ^ {2} / (2 k + 1).
$$

There is bug that one has to avoid: by dividing the last term twice by p and a third time by 2k 1 the variable imin is updated. For the next term we need to know the value of imin before the division by 2k 1! Otherwise we will get erroneous results when forming $t _ { k } / p ^ { 2 }$ 

## Solution:

For the subtraction of two multiple precision numbers we propose 

```matlab
function r=Sub(c,a,b)
% SUB computes r=a-b where a and b are multiprecision numbers
% with a>b.
n=length(a);
r=a;
for i=n:-1:1
    while a(i)<b(i) % need to borrow from left
    a(i)=a(i)+c; b(i-1)=b(i-1)+1;
    end
    r(i)=a(i)-b(i);
end 
```

We reuse the functions Divide, Add and Carry. The multiprecision function for arctan becomes 

```matlab
function s=AtanMultPrec(c,n,p)
% ATANMULTPREC computes n*log10(c) decimal digits
% of the function value s=arctan(1/p) where p>1 is
% an integer number
s=zeros(1,n,'uint32');
s(1)=1;
imin=0;    % imin counts leading zeros in t
[s,imin]=Divide(c,imin,p,s);    % s=1/p
t=s;    % first term
k=1;
sig=1;    % the sign of the term
while imin<n
    k=k+2;
    [t,imin]=Divide(c,imin,p^2,t);% new nominator of term 
```

```matlab
h=Divide(c,imin,k,t); % division without change of imin
sig=-sig; % change sign
switch sig
case -1
s=Sub(c,s,h); % subtract or
case 1
s=Add(imin,s,h); % add term h to s
s=Carry(c,s);
end
end 
```

Finally we compute π by the function 

```matlab
function s=Pi(c,n)
% PI computes n decimal digits of pi using the
% formula of Stormer.
s=24*AtanMultPrec(c,n,8); % generate the 3 terms
t2=8*AtanMultPrec(c,n,57);
t3=4*AtanMultPrec(c,n,239);
s=Add(1,s,t2); % add the terms
s=Add(1,s,t3);
s=Carry(c,s);
sprintf('%01d',s) 
```

## and get for n 1000

<table><tr><td>&gt;&gt; tic, Pi(10,1000); tocans =3141592653589793238462643383279502884197169399375105820974944592307816406286208998628034825342117067982148086513282306647093844609550582231725359408128481117450284102701938521105559644622948954930381964428810975665933446128475648233786783165271201909145648566923460348610454326648213393607260249141273724587006606315588174881520920962829254091715364367892590360011330530548820466521384146951941511609433057270365759591953092186117381932611793105118548074462379962749567351885752724891227938183011949129833673362440656643086021394946395224737190702179860943702770539217176293176752384674818467669405132000568127145263560827785771342757789609173637178721468440901224953430146549585371050792279689258923542019956112129021960864034418159813629774771309960518707211349999998372978049951059731732816096318595024459455346908302642522308253344685035261931188171010003137838752886587533208381420617177669147303598253490428755468731159562863882353787593751957781857780532171226806613001927876611195909216419964</td></tr></table>

```txt
Elapsed time is 35.828138 seconds. 
```

## 10.6 Chapter 6: Solving Linear Equations

1. LU-decomposition Consider the linear system Ax b defined by the matrix 

```erlang
>> format short e, format compact
>> n=5; A=invhilb(n), b=eye(n,1) 
```

(a) Apply Gaussian Elimination (without pivoting) to reduce the system to Ux y 

```matlab
for j=1:n-1 % Elimination
    for k=j+1:n
    fak=A(k,j)/A(j,j);
    A(k,j:n)=A(k,j:n)-fak*A(j,j:n);
    b(k)=b(k)-fak*b(j);
    end
end 
```

Watch the elimination process by displaying the matrix and the right hand side after each elimination step. Use the pause statement to stop execution. 

Solution: 

```matlab
for j=1:n-1 % Elimination
    for k=j+1:n
    fak=A(k,j)/A(j,j);
    A(k,j:n)=A(k,j:n)-fak*A(j,j:n);
    b(k)=b(k)-fak*b(j);
    end
    [A, b] % display A and b
    pause % wait for ret
end 
```

We observe the elimination process and get at the end 

```txt
>> A
A =
25 -300 1050 -1400 630
0 1200 -6300 10080 -5040
0 0 2205 -5880 3780
0 0 0 448 -504
0 0 0 0 9
>> b
b =
1.0000
12.0000
21.0000
11.2000
1.8000 
```

We see the reduction of A to an upper triangular matrix U. 

(b) Next store the factors fak instead of the zeros you introduce by eliminating x <sub>j</sub> : 

```matlab
for j=1:n-1 % Elimination
    for k=j+1:n
    fak=A(k,j)/A(j,j);
    A(k,j)=fak; % store factors instead zeros
    A(k,j+1:n)=A(k,j+1:n)-fak*A(j,j+1:n);
    end
end 
```

Now use the commands triu, tril, diag to extract L and U from A and verify that indeed LU A. 

Solution: The second version of Gaussian Elimination stores the factors used for elimination where we would produce the zeros. Notice the difference 

```matlab
A(k,j:n)=A(k,j:n)-fak*A(j,j:n); % first version
A(k,j+1:n)=A(k,j+1:n)-fak*A(j,j+1:n); % second version 
```

Now we get the results 

```csv
A =
2.5000e+01 -3.0000e+02 1.0500e+03 -1.4000e+03 6.3000e+02
-1.2000e+01 1.2000e+03 -6.3000e+03 1.0080e+04 -5.0400e+03
4.2000e+01 -5.2500e+00 2.2050e+03 -5.8800e+03 3.7800e+03
-5.6000e+01 8.4000e+00 -2.6667e+00 4.4800e+02 -5.0400e+02
2.5200e+01 -4.2000e+00 1.7143e+00 -1.1250e+00 9.0000e+00 
```

The reduced matrix U is still in the upper part and can be extracted by 

$$
\begin{array}{l l l l l} \text {>> U = triu(A)} \\ \mathrm{U=} \\ 2 5 & - 3 0 0 & 1 0 5 0 & - 1 4 0 0 & 6 3 0 \\ 0 & 1 2 0 0 & - 6 3 0 0 & 1 0 0 8 0 & - 5 0 4 0 \\ 0 & 0 & 2 2 0 5 & - 5 8 8 0 & 3 7 8 0 \\ 0 & 0 & 0 & 4 4 8 & - 5 0 4 \\ 0 & 0 & 0 & 0 & 9 \end{array}
$$

The function triu is an abbreviation for “upper triangle”. The matrix L is constructed from the factors we stored instead of the zeros. With 

```txt
>> L=tril(A)
L =
1.0e+03 *
0.0250    0    0    0    0
-0.0120    1.2000    0    0    0
0.0420    -0.0053    2.2050    0    0
-0.0560    0.0084    -0.0027    0.4480    0
0.0252    -0.0042    0.0017    -0.0011    0.0090 
```

we get the lower triangle of A including the diagonal. We need now to replace the diagonal by all number 1. The function diag is useful for that. With 

```txt
>> D=diag(L)
D =
25
1200
2205
448
9 
```

we extract the diagonal as a vector. If we use diag with a vector as argument then a diagonal matrix is produced: 

<table><tr><td colspan="5">&gt;&gt; D=diag(D)</td></tr><tr><td>D =</td><td></td><td></td><td></td><td></td></tr><tr><td>25</td><td>0</td><td>0</td><td>0</td><td>0</td></tr><tr><td>0</td><td>1200</td><td>0</td><td>0</td><td>0</td></tr><tr><td>0</td><td>0</td><td>2205</td><td>0</td><td>0</td></tr><tr><td>0</td><td>0</td><td>0</td><td>448</td><td>0</td></tr><tr><td>0</td><td>0</td><td>0</td><td>0</td><td>9</td></tr></table>

Now we can form 

$$
\begin{array}{r l} & \text { >>   L = L - D + eye(5) } \\ & \text { L = } \\ & 1. 0 0 0 0 \quad 0 \quad 0 \quad 0 \quad 0 \\ & - 1 2. 0 0 0 0 \quad 1. 0 0 0 0 \quad 0 \quad 0 \quad 0 \\ & 4 2. 0 0 0 0 \quad - 5. 2 5 0 0 \quad 1. 0 0 0 0 \quad 0 \quad 0 \\ & - 5 6. 0 0 0 0 \quad 8. 4 0 0 0 \quad - 2. 6 6 6 7 \quad 1. 0 0 0 0 \quad 0 \\ & 2 5. 2 0 0 0 \quad - 4. 2 0 0 0 \quad 1. 7 1 4 3 \quad - 1. 1 2 5 0 \quad 1. 0 0 0 0 \end{array}
$$

So to summarize we just have to write 

```c
>> U=triu(A); % decompose A, upper part
>> L=tril(A); % extract lower triangular matrix
>> L=L-diag(diag(L))+eye(size(L)); % adjust diagonal
>> L*U
ans =
25 -300 1050 -1400 630
-300 4800 -18900 26880 -12600
1050 -18900 79380 -117600 56700
-1400 26880 -117600 179200 -88200
630 -12600 56700 -88200 44100 
```

and we get L<sub>*</sub>U=A as expected. 

2. Replace the computation of the rotation matrix S in our function EliminationGivens by the Matlab-function planerot. Convince yourself that you get the same results with the modified function by solving the curve fitting example again. 

## Solution:

```matlab
function x=EliminationGivens2(A,b);
% ELIMINATIONGIVENS solves a linear system using Givens-rotations
% x=EliminationGivens(A,b) solves Ax=b using Givens-rotations. 
```

```matlab
[m,n]=size(A);
for i=1:n
    for k=i+1:m
    if A(k,i)~=0
    [S,y] = planerot([A(i,i);A(k,i)]);
    A(i,i)=y(1);
    A(i:k-i:k,i+1:n)=S*A(i:k-i:k,i+1:n);
    b(i:k-i:k)=S*b(i:k-i:k);
    end
    end;
    if A(i,i)==0
    error('Matrix is rank deficient');
    end;
end
x=zeros(n,1);
for k=n:-1:1 % backsubstitution
    x(k)=(b(k)-A(k,k+1:n)*x(k+1:n))/A(k,k);
end
x=x(:); 
```

Indeed by replacing EliminationGivens by EliminationGivens2 in CurveFit we get the same results. 

3. Determine the parameters a and b such that the function $f ( x ) = a e ^ { b x }$ fits the following data 

```txt
x 30.0 64.5 74.5 86.7 94.5 98.9
y 4 18 29 51 73 90 
```

Plot the points and the fitted function. 

Hint: If you fit log f(x) the problem becomes very easy! 

Solution: Taking the logarithm of the function we get 

$\ln y = \ln a + bx.$ 

With the unknown c  ln a the least squares problem becomes 

$$
\left( \begin{array}{c c} 1 & 3 0. 0 \\ 1 & 6 4. 5 \\ 1 & 7 4. 5 \\ 1 & 8 6. 7 \\ 1 & 9 4. 5 \\ 1 & 9 8. 9 \end{array} \right) \binom{c}{b} \approx \left( \begin{array}{c} \ln 4 \\ \ln 1 8 \\ \ln 2 9 \\ \ln 5 1 \\ \ln 7 3 \\ \ln 9 0 \end{array} \right).
$$

```matlab
% Problem 6_4_1
clear, clf
x=[30.0, 64.5, 74.5, 86.7, 94.5, 98.9]';
y=[4, 18, 29, 51, 73, 90]';
A=[ones(size(x)), x] 
```

```matlab
b=log(y);
p=A\b
a=exp(p(1))
b=p(2)
plot(x,y,'o')
hold
z=[30:100];
plot(z, a*exp(b*z)) 
```

The solution is 

$$
b = 0. 0 4 5 2 4 3 1 0 6 4 8 \text {   and   } c = 0. 0 0 7 8 9 2 6 2 4 0 6 \Rightarrow a = 1. 0 0 7 9 2 7 5 2.
$$

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/65f72ba7f2bada22ba44e6017019919a2f126729150f9afc64f95e3303b92b70.jpg)



4. The following statistics lists the population of Shanghai since 1953:


<table><tr><td colspan="2">year in million</td></tr><tr><td>1953</td><td>6.2044</td></tr><tr><td>1964</td><td>10.8165</td></tr><tr><td>1982</td><td>11.8597</td></tr><tr><td>1990</td><td>13.3419</td></tr><tr><td>2000</td><td>16.4077</td></tr><tr><td>2010</td><td>23.0192</td></tr></table>

Fit a polynomial through these data and predict the population for 2016 and 2020. Plot your results. 

## Solution:

Matlab provides the functions polyfit to fit a polynomial through points and polyval to evaluate a polynomial at some points. Thus the problem is readily solved: 

```matlab
x=[1953 1964 1982 1990 2000 2010]'
y=[6.2044 10.8165 11.8597 13.3419 16.4077 23.0192]'
p=polyfit(x,y,5) % Interpolate by polynomial of deg. 5
xx=[x;2016; 2020] % add extrapolation points
yy=[y;polyval(p,[2016 2020])']% extrapolate
plot(xx,yy,'*') 
```

We get the result 31.5600 millions for 2014 and 40.8764 millions for 2020. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/84e09167988a5db4b08a269b6c3c5fa97442cc2ed1b2127ccbfe8b0bcaf8b341.jpg)


Without using the above mentioned functions we have to compute the coefficients of the interpolating polynomial by solving the system: 

$$
\begin{array}{c} p _ {1} x _ {1} ^ {5} + p _ {2} x _ {1} ^ {4} + \dots + p _ {5} x _ {1} + p _ {6} = y _ {1} \\ p _ {1} x _ {2} ^ {5} + p _ {2} x _ {2} ^ {4} + \dots + p _ {5} x _ {2} + p _ {6} = y _ {2} \\ \vdots \qquad \qquad \qquad \qquad \vdots \quad \vdots \\ p _ {1} x _ {6} ^ {5} + p _ {2} x _ {6} ^ {4} + \dots + p _ {5} x _ {6} + p _ {6} = y _ {6} \end{array}
$$

The matrix is a Vandermonde matrix. It can be generated by 

$$
A = [ x. ^ {\wedge} 5, x. ^ {\wedge} 4, x. ^ {\wedge} 3, x. ^ {\wedge} 2, x, \text { ones } (\text { size } (x)) ]
$$

So the coefficients are obtained by p=A y. Indeed we get 

```txt
>> A=[x.^5, x.^4, x.^3, x.^2, x, ones(size(x))]
A =
1.0e+16 *
2.8413 0.0015 0.0000 0.0000 0.0000 0.0000
2.9222 0.0015 0.0000 0.0000 0.0000 0.0000
3.0586 0.0015 0.0000 0.0000 0.0000 0.0000
3.1208 0.0016 0.0000 0.0000 0.0000 0.0000
3.2000 0.0016 0.0000 0.0000 0.0000 0.0000
3.2808 0.0016 0.0000 0.0000 0.0000 0.000 
```

```txt
Warning: Matrix is close to singular or badly scaled. Results may be inaccurate.
RCOND = 2.726773e-28. 
```

```csv
p =
1.0e+09 *
0.0000
-0.0000
0.0000
-0.0000
0.0222
-8.7968 
```

To evaluate the polynomial we write the function 

```matlab
function y=EvalPoly(p,x)
n=length(p);
y=0;
for i=1:n
    y=y*x+p(i);
end 
```

and we obtain the same results as before: 

```txt
>> y=EvalPoly(p,2016)
y =
31.5602
>> y=EvalPoly(p,2020)
y =
40.8768 
```

Remark: The solution is numerically not optimal. It is not good to evaluate a polynomial in standard form for a few values far away from the origin. A numerically better solution would be to make a shift and to work with the polynomial 

$$
p (x) = p _ {1} (x - 1 9 8 0) ^ {5} + p _ {2} (x - 1 9 8 0) ^ {4} + \dots + p _ {6}.
$$

5. Fitting ofcircles. We are given the measured points $( \xi _ { i } , \eta _ { i } )$ 

$$
\begin{array}{c c c c c c c c c} \xi & 0. 7 & 3. 3 & 5. 6 & 7. 5 & 6. 4 & 4. 4 & 0. 3 & - 1. 1 \\ \hline \eta & 4. 0 & 4. 7 & 4. 0 & 1. 3 & - 1. 1 & - 3. 0 & - 2. 5 & 1. 3 \end{array}
$$

Find the center $( c _ { 1 } , c _ { 2 } )$ and the radius r of a circle $( x - c _ { 1 } ) ^ { 2 } + ( y - c _ { 2 } ) ^ { 2 } = r ^ { 2 }$ that approximate the points as well as possible. Consider the algebraicfit: Rearrange the equation of the circle as 

$$
2 c _ {1} x + 2 c _ {2} y + r ^ {2} - c _ {1} ^ {2} - c _ {2} ^ {2} = x ^ {2} + y ^ {2}.\tag{10.1}
$$

With $w = r ^ { 2 } - c _ { 1 } ^ { 2 } - c _ { 2 } ^ { 2 }$ , we obtain with (6.7) for each measured point a linear equation for the unknowns $c _ { 1 } , c _ { 2 }$ and $w$ . 

Write a function function drawcircle $\left( \mathbf { C } , \mathbf { r } \right)$ to plot a circle with center $\left( \mathbf { C } \left( \ 1 \right) , \mathbf { C } \left( \ 2 \right) \ \right)$ and radius r. 

Computer the center and the radius and plot the given points and the fitted circle. 

## Solution:

```matlab
We first write a function to plot a circle

function drawcircle(C,r,w);
% draws a circle with center (C(1), C(2)) and radius r
if nargin==2, w = '-'; end
theta = [0:0.02:2*pi];
plot(C(1)+r*cos(theta), C(2)+r*sin(theta),w);
plot(C(1),C(2),'x');

The main program is straightforward:
xi = [ 0.7 3.3 5.6 7.5 6.4 4.4 0.3 -1.1 ];
eta = [ 4.0 4.7 4.0 1.3 -1.1 -3.0 -2.5 1.3 ];
A = [2*pi 2*eta ones(size(xi))]
b=xi.^2+eta.^2;
x = A\b
C=x(1:2)
r=sqrt(x(3)+C(1)^2+C(2)^2)
plot(xi,eta,'o')
axis equal
hold
drawcircle(C,r)

The results are
C =
    3.060303565727350
    0.743607321042322
>> r
r =
    4.109137036074778 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/0815825b6b663cfdd4b2585dd3230187b8529107ca5ef1cbc7c94d29d568d873.jpg)


6. Seven dwarfs are sitting around a table. Each one has a cup. The cups contain milk, all together a total of 3 liter. One of the dwarfs starts distributing his milk evenly over all cups. After he has finished his right neighbor does the same. Clockwise the next dwarfs proceed distributing their milk. After the 7th dwarf has distributed his milk, there is in each cup as much milk as at the beginning. How much milk was initially in each cup? 

Hint: Let $\pmb { x } = ( x _ { 1 } , x _ { 2 } , \ldots , x _ { 7 } ) ^ { \top }$ be the initial milk distribution. Thus $\textstyle \sum _ { j = 1 } ^ { 7 }$ $x _ { j } = 3$ . Simulate the distributing of milk as matrix-vector Operation: 

$$
\boldsymbol {x} ^ {(1)} = T _ {1} \boldsymbol {x}.
$$

After 7 distributions you obtain $\mathbf { x } ^ { ( 7 ) } = \mathbf { x }$ and thus 

$$
\boldsymbol {x} = T _ {7} T _ {6} \dots T _ {1} \boldsymbol {x}
$$

or $( A - I ) { \pmb x } = 0$ where $A = T _ { 7 } T _ { 6 } \cdot \cdot \cdot T _ { 1 }$ . Add to this homogeneous system the equation $\begin{array} { r } { \sum _ { j = 1 } ^ { 7 } x _ { j } = 3 } \end{array}$ and solve the system using our function Elimination Givens. Compare the results you get with those when using Matlab’s - operator. 

Solution: Let 

$$
x _ {1} ^ {(0)}, \dots , x _ {7} ^ {(0)} \text {   be   the   initial   milk   amounts   }
$$

and let 

$x _ { 1 } ^ { ( 1 ) } , \ldots , x _ { 7 } ^ { ( 1 ) }$ the amounts after the first distribution. 

We have 

$$
\pmb {x} ^ {(1)} = T ^ {(1)} \pmb {x} ^ {(0)},
$$

where 

$$
T ^ {(1)} = \left( \begin{array}{c c c c c} 1 / 7 & 0 & \dots & & 0 \\ 1 / 7 & 1 & 0 & \dots & 0 \\ 1 / 7 & 0 & 1 & \ddots & \vdots \\ \vdots & \vdots & \ddots & \ddots & 0 \\ 1 / 7 & 0 & \dots & 0 & 1 \end{array} \right).
$$

The ith distribution is given by the transformation 

$$
\pmb {x} ^ {(i)} = T ^ {(i)} \pmb {x} ^ {(i - 1)}
$$

where $T ^ { ( i ) }$ looks like $T ^ { ( 1 ) }$ only the column with the elements $1 / 7$ is now the ith column instead of the first. For the final state we have 

$$
\boldsymbol {x} ^ {(7)} = \underbrace {T ^ {(7)} \cdots T ^ {(1)}} _ {A} \boldsymbol {x} ^ {(0)}
$$

and since $\pmb { x } ^ { ( 7 ) } = \pmb { x } ^ { ( 0 ) } = : \pmb { x }$ we obtain the homogeneous linear system 

$$
(A - I) \boldsymbol {x} = 0.
$$

One can prove that a non-trivial solutions exist. The solution is unique if we consider the total amount of milk and if we add the equation 

$$
x _ {1} + x _ {2} + \dots + x _ {7} = 3
$$

to the system. 

```matlab
% Dwarfs Milk Distribution Problem
I=eye(7);
e=ones(7,1);
e7=e/7;
A=I;
for k=1:7
    T=I;    % construct T_i
    T(:,k)=e7;
    A=T*A;
end
B=[A-I; e'];
b=[zeros(size(e));3];    % add total amount of milk
x=B\b

Check = A*x
x =
    0.7500
    0.6429
    0.5357
    0.4286
    0.3214
    0.2143
    0.1071 
```

7. The following sections were measured on the street $\overline { { A D } }$ depicted in Fig. 6.1 (Fig. 10.2). 

$$
\mathrm{AD} = 8 9 \mathrm{m}, \mathrm{AC} = 6 7 \mathrm{m}, \mathrm{BD} = 5 3 \mathrm{m}, \mathrm{AB} = 3 5 \mathrm{m} \text { and } \mathrm{CD} = 2 0 \mathrm{m}
$$

Balance out the measured sections using the least squares method. 

<table><tr><td>A</td><td>B</td><td>C</td><td>D</td></tr></table>


Fig. 10.2 Street


Solution: 

Let $x _ { 1 } = { \overline { { A B } } } , x _ { 2 } = { \overline { { B C } } }$ and $x _ { 3 } = \overline { { C D } }$ . The measurements lead to the equations 

$$
\begin{array}{c} x _ {1} + x _ {2} + x _ {3} = 8 9 \\ x _ {1} + x _ {2} = 6 7 \\ x _ {2} + x _ {3} = 5 3 \iff A \boldsymbol {x} = \boldsymbol {b}, \quad A = \left( \begin{array}{c c c} 1 & 1 & 1 \\ 1 & 1 & 0 \\ 0 & 1 & 1 \\ 1 & 0 & 0 \\ 0 & 0 & 1 \end{array} \right), \quad \boldsymbol {b} = \left( \begin{array}{c} 8 9 \\ 6 7 \\ 5 3 \\ 3 5 \\ 2 0 \end{array} \right) \\ x _ {1} = 3 5 \\ x _ {3} = 2 0 \end{array}
$$

Solving the system with the -operator we get 

```txt
>> A = [1 1 1; 1 1 0; 0 1 1; 1 0 0; 0 0 1];
>> b = [89; 67; 53; 35; 20];
>> x = A\b
x =
35.1250
32.5000
20.6250 
```

We obtain the same result with our function EliminationGivens: 

```txt
>> x=EliminationGivens(A,b)
x =
35.1250
32.5000
20.6250 
```

## 10.7 Chapter 7: Recursion

1. Cramer’s Rule for solving systems of linear equations. This rule is often used when solving small $( n \leq 3 )$ systems of linear equations by hand. 

Write a function x=Cramer(A,b) which solves a linear system Ax b using Cramer’s rule. For det $( A ) \neq 0$ , the linear system has the unique solution 

$$
x _ {i} = \frac {\det (A _ {i})}{\det (A)}, \quad i = 1, 2, \dots , n,\tag{10.2}
$$

where $A _ { i }$ is the matrix obtained from A by replacing column $\pmb { a } : i$ by b. Use the function DetLaplace to compute the determinants. 

Test your program by generating a linear system with known solution. 

## Solution:

```matlab
function x=Cramer(A,b);
% CRAMER solves a linear System with Cramer's rule
% x=Cramer(A,b); Solves the linear system Ax=b using Cramer's 
```

% rule. The determinants are computed using the function DetLaplace. 

```matlab
n=length(b);
detA=DetLaplace(A);
for i=1:n
    AI=[A(:,1:i-1), b, A(:,i+1:n)];
    x(i)=DetLaplace(AI)/detA;
end
x = x(:);

>> A=rand(7,7);
>> x=[1:7]';
>> b=A*x;
>> xx=Cramer(A,b);
>> norm(x-xx)
ans =
    1.1997e-13 
```

## 2. Selection Sort versus Quick Sort.

The idea of selection sort is to find the minimum value in the given array and then swaps it with the value in the first position. By repeating this for the remaining elements the array is sorted. 

(a) Write a (non-recursive) function a=SelectSort(a) which implements the Selection Sort. Show the process using bar and pause as done in Quick Sort. Test your program by sorting some small arrays (n 100) 

Solution: 

```matlab
function a = SelectionSort(a)
n=length(a);
for i=1:n-1
    [amin,k]=min(a(i:n)); k=k+i-1;
    if k~=i % swap
    h=a(k); a(k)=a(i); a(i)=h;
    % bar(a); pause(0.01)
    end
end 
```

(b) Speed Test: Remove the bar and pause statement in both functions and measure the time each function needs to sort an array of 100’000 elements. Use for this the Matlab-functions tic and toc. 

Solution: We comment out the line in both functions with the statements bar(a); pause(0.01) and run the main program 

```matlab
% speed test
clear
global a
n=100000
aa=rand(1,n);
a=aa; tic, a=SelectionSort(a); toc
a=aa; tic, quick(1,n); toc 
```

We get on our laptop the result 

```txt
>> SpeedTest
n =
100000
Elapsed time is 13.458101 seconds.
Elapsed time is 1.511749 seconds. 
```

Clearly quick wins over SelectionSort. 

(c) For fun (not efficient!): program the selection sort recursively. Use a global array and proceed similarly as with quicksort. 

Solution: We need a main program which defines the global array a: 

```matlab
% SelectionSortMain.m
global a
n=50
a=rand(1,n);
bar(a)
pause
SelectionSortRec(1,n)
bar(a) 
```

The recursive function SelectionSortRec is designed similarly like quick. However, it is very inefficient since it is a single recursion. For n elements we need also n recursive calls! 

```matlab
function SelectionSortRec(left, n)
global a
if left < n,
    [amin, k] = min(a(left: n));
    k = k + left - 1;
    if k ~ = left % swap
    h = a(k); a(k) = a(left); a(left) = h;
    end
    bar(a); pause(0.01)
    left = left + 1;
    SelectionSortRec(left, n);
end 
```

3. Pythagoras Tree<sup>1</sup>: 

Basic construction: Given two points P and Q in the plane, construct the points P and Q to built a square. Then put on the square a right triangle with one basis angle α. 

The following figure shows the basic construction and the first recursion step, where the construction is repeated on top of the cathetes of the triangle P R Q . 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/40212a8fb8c930973a28fdee6c792ba1f0f32271c5e39276d6838aa3ebd590b7.jpg)


Write a recursive function which computes the Pythagoras tree until the base line P Q becomes small. Experiment with the basis angle, choose e.g. as here in the figure <sub>α</sub> 20◦. 

Solution: Recursive function: 

```matlab
function ptree(P,Q,alpha)
% PTREE constructs a Pythagorean tree
% ptree(P,Q,alpha) plots a Pythagorean tree over the basis line given by the
% two points P=(p1,p2) an Q=(q1,q2) in the plane with a right triangle
% with one basis angle alpha (in degrees)

g=norm(P-Q); % length of square
r=Q-P; r=r/norm(r); % direction vector
n=[-r(2), r(1)]; % normal vector
Ps=P+n*g; Qs=Q+n*g; % other corners of square
X=[P;Q;Qs;Ps;P]';
plot(X(1,:), X(2,:)) % draw the square

c=cos(alpha); s=sin(alpha);
Rot=[c s;-s c]; % rotation matrix Rot
R=Ps+r*Rot*g*c; % construct triangle Ps-R-Qs over Ps-Qs
Y=[Ps;R;Qs]';
% draw triangle
plot(Y(1,:), Y(2,:))
if g>0.1 % recursion for both sides
    ptree(Ps,R,alpha); % of triangle 
```

```julia
ptree(R, Qs, alpha)
end 
```

Main program: 

```matlab
% Mainprogram Mainptree.m
% recursive Pythagoras tree
% example of a fractal
clf
axis([-25,15,-5,35])
axis square
hold
alpha=input('angle=? (degrees)')
ptree([1,1],[5,0],alpha*pi/180) 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/e62ba8fedbda0225f0a59f50eeab155fa5162cd1b0585f0a01b563d5cf243fa4.jpg)


4. Permutations: Matlab has the function perms to compute permutations. For instance 

```txt
>> a=[1 2 3]
a =
    1    2    3
>> perms(a)
ans =
    3    2    1
    3    1    2
    2    3    1
    2    1    3
    1    2    3
    1    3    2 
```

displays all 6 permutations of the three numbers. 

Write a recursive function Permute(n) which does the same. Choose the array a as global variable. 

## Solution:

```matlab
function Permute(k)
global a Z
if k==1 % finish recursion
    Z=[Z;a]; % and store permutation
else
    Permute(k-1); % permute a_1, ..., a_{k-1}
    for i=1:k-1
    t=a(i); a(i)=a(k); a(k)=t; % exchange a_i <-> a_k
    Permute(k-1) % and permute
    t=a(i); a(i)=a(k); a(k)=t; % exchange back
    end
end

Indeed we get with
% MainPermute.m
global a Z
a=[1 2 3]
Z=[];
Permute(3)
Z

>> MainPermute
a =
    1    2    3
Z =
    1    2    3
    2    1    3
    3    2    1
    2    3    1
    1    3    2
    3    1    2 
```

## 10.8 Chapter 8: Iteration and Nonlinear Equations

1. Bisection-Algorithm. Improve the function Bisekt. Your function [x,y]= Bisection(f,a,b,tol) should also compute a zero for functions with f(a) > 0 and f(b) < 0 to a given tolerance tol. Be careful to stop the iteration in case the user asks for a too small tolerance! If by the bisection process we arrive at an interval (a, b) which does not contain a machine number anymore then it is high time to stop the iteration. 

## Solution:

```matlab
function [x,y]=Bisection(f,a,b,tol)
% BISECTION computes a root of a scalar equation
%    [x,y]=Bisection(f,a,b,tol) finds a root x of the scalar function
%    f in the interval [a,b] up to a tolerance tol. y is the
%    function value at the solution

fa=f(a); v=1; if fa>0, v=-1; end;
if fa*f(b)>0
    error('f(a) and f(b) have the same sign')
end
if (nargin<4), tol=0; end;
x=(a+b)/2;
while (b-a>tol) & ((a<x) & (x<b))
    if v*f(x)>0, b=x; else a=x; end;
    x=(a+b)/2;
end
if nargout==2, y=f(x); end; 
```

## 2. Solve with bisection the equations

(a) $x^{x}=50$ (b) $\ln(x)=\cos(x)$ (c) $x+e^{x}=0$ . 

Hint: a starting interval is easy to find by sketching the functions involved. 

## Solution:

(a) The function x<sup>x</sup> is monotonically increasing. Since 1<sup>1</sup> 1 and 4<sup>4</sup> 256 the values a 1 and b 4 can be used for the bisection. The solution becomes 

```txt
>> [x,f]=Bisection(@(x) x^x-50,1,4)
x =
3.287262195355581
f =
7.105427357601002e-15 
```

(b) Drawing the functions ln(x) and cos(x) we see that their cutting point is in the interval (0, /2), thus 

```txt
>> [x,f]=Bisection(@(x) log(x)-cos(x),0,pi)
x =
1.302964001216012
f =
-2.220446049250313e-16 
```

(c) We write the equation e<sup>x</sup> x and from the graph of the two functions we get the interval ( 1, 0) for the solution, so 

```diff
>> [x,f]=Bisection(@(x) exp(x)+x,-1,0)
x =
-0.567143290409784
f =
-1.110223024625157e-16 
```

3. Find x such that 

$$
\int_ {0} ^ {x} e ^ {- t ^ {2}} d t = 0. 5.
$$

Hint: the integral cannot be evaluated analytically, so expand it in a series and integrate. Write a function $\boldsymbol { \mathrm { \Sigma } } ( \boldsymbol { \mathrm { x } } )$ to evaluate the series. Then use bisection to compute the solution of $f ( x ) - 0 . 5 = 0$ 

## Solution:

Take the series for $e ^ { x }$ , substitute $x = - t ^ { 2 }$ and integrate to get the expansion 

$$
\int_ {0} ^ {x} e ^ {- t ^ {2}} d t = x - \frac {x ^ {3}}{1 ! 3} + \frac {x ^ {5}}{2 ! 5} - \frac {x ^ {7}}{3 ! 7} + \frac {x ^ {9}}{4 ! 9} \mp \dots\tag{10.3}
$$

For evaluating the series we introduce the expressions 

$$
t a := (- 1) ^ {i - 1} \frac {x ^ {2 i - 1}}{(i - 1) !} \quad t := (- 1) ^ {i} \frac {x ^ {2 i + 1}}{i !}
$$

then $t = - t a * x ^ { 2 } / i$ and the partial sum is updated by $s _ { \mathrm { n e w } } = s _ { \mathrm { o l d } } + t / ( 2 * i + 1 )$ We will stop the summation when $s _ { \mathrm { n e w } } = s _ { \mathrm { o l d } }$ . Thus we get 

```matlab
function y=ff(x);
% is used in IntegralExp.m
t=x; snew=x; sold=0; i=0;
while sold ~= snew
    i=i+1;
    sold=snew;
    t=-t*x^2/i;
    snew=sold+t/(2*i+1);
end
y=snew;

>> [x,f]=Bisection(@(x) ff(x)-0.5,0,1)
x =
    0.551039427609027
f =
    0 
```

4. Use bisection to create the following table: 

<table><tr><td>F</td><td>0</td><td><eq>0.1\pi</eq></td><td><eq>0.2\pi</eq></td><td>...</td><td><eq>\pi</eq></td></tr><tr><td>h</td><td>0</td><td>?</td><td>?</td><td>...</td><td>2</td></tr></table>

where the function F(h) is given by 

$$
F (h) = \pi - 2 \arccos \frac {h}{2} + h \sqrt {1 - \left(\frac {h}{2}\right) ^ {2}}.
$$

Solution: To compute the table entries we loop through the values $0 : 0 . 1 \pi : \pi$ The equation to be solved by bisection changes during the loop. A simple way to deal with this is to use a global variable. The main program becomes: 

```matlab
% Table.m
global f
format long
res=[];
for f=0:0.1*pi:pi;
    [x y]=Bisection(@F,0,2);
    res=[res; f x y];
end;
res
and the function is
function z=F(h)
global f
z=pi-2*acos(h/2.0)+h.*sqrt(1-(h/2).^2)-f; 
```

Running the program we obtain 

```csv
res =
0 0 0
0.314159265358979 0.157241774836456 0.000000000000000
0.628318530717959 0.315472387600032 0
0.942477796076938 0.475764878639765 -0.000000000000000
1.256637061435917 0.639383019581008 0.000000000000000
1.570796326794897 0.807945506599034 -0.000000000000000
1.884955592153876 0.983723665527420 0.00000000000000
2.199114857512855 1.170274845761590 0
2.513274122871834 1.374097652265081 0.0000000000000
2.827433388230814 1.610767273040240 0
3.141592653589793 2.000000000000 
```

5. Binary search: we are given an ordered sequence of numbers: 

$$
x _ {1} \leq x _ {2} \leq \dots \leq x _ {n}
$$

and a new number z. Write a program that computes an index value i such that either $x _ { i - 1 } < z \leq x _ { i }$ or i 1 or i n 1 holds. The problem can be solved by considering the function 

$$
f (i) = x _ {i} - z
$$

and computing its “zero” by bisection. 

Solution: 

```matlab
function Binsearch(z,x)
n=length(x);
if z<x(1),
    disp(strcat('z = ',num2str(z),' is smaller than x(1) = ',num2str(x(1))))
elseif z>x(n),
    disp(strcat('z = ',num2str(z),' is larger than x(n) = ',num2str(x(n))))
else
    a=1; b=n;
    while a+1~=b
    i=round((a+b)/2);
    if x(i)<z; a=i;
    else b=i;
    end
    end
    i=b;
    disp(strcat('i = ',num2str(i),' and ',' z = ',num2str(z),' is in [',... num2str(x(a)),','', 'num2str(x(b)),']'))
end 
```

We test this function with the main program 

```matlab
% MainBinSearch.m
x=[-1.4 0 3.7 5.1 7.9 9.4 11.6 13.1 17 25.4 26]'
for z=[8, 17.5, -3, 32]
    BinSearch(z,x)
end

>> MainBinSearch
x =
    -1.4000
    0
    3.7000
    5.1000
    7.9000
    9.4000
    11.6000
    13.1000
    17.0000
    25.4000
    26.0000
i =6 and z =8 is in [7.9,9.4]
i =10 and z =17.5 is in [17,25.4]
z =-3 is smaller than x(1) =-1.4
z =32 is larger than x(n) =26 
```

6. Compute x where the following maximum is attained: 

$\max_{0 < x < \frac{\pi}{2}}\left(\frac{1}{4\sin x} +\frac{\sin x}{2x} -\frac{\cos x}{4x}\right).$ 

Solution: We differentiate and compute the zero of the derivative using bisection. We choose for a 0.001 since with a 0 the denominator is zero 

## 10.8 Chapter 8: Iteration and Nonlinear Equations

```txt
>> Bisection(@(x) cos(x)/4/x*(2-x/(sin(x))^2+1/x)+...
    sin(x)/4/x*(1-2/x),0.001,pi/2)
ans =
1.031158096685125 
```

7. Write a function s=SquareRoot(a) which computes the square root using Heron’s algorithm. Think of a good starting value and a good termination criterion. 

Hint: consider the geometrical interpretation of Newton’s method and use the (theoretical) monotonicity of the sequence as termination criterion. 

Test your function and compare the results with the standard Matlab-function sqrt. Compute the relative error of both functions 

## Solution:

```matlab
function s = SquareRoot(a);
% SQUAREROOT computes the square root
% using Heron's algorithm
xold = (1+a)/2; xnew = (xold + a / xold) / 2;
while xnew < xold % as long as monotone
    xold = xnew; xnew = (xold + a / xold) / 2;
end
s = xnew; 
```

## With the testprogram

```matlab
% TestSquareRoot.m
z = [];
for x = 1:10:1000
    z = [z; x (SquareRoot(x) - sqrt(x)) / sqrt(x)];
end
for i = 1:30
    fprintf('%10d %15.6e %10d %15.6e %10d %15.6e\n', z(i,1),z(i,2), ...
    z(i+30,1),z(i+30,2), z(i+60,1),z(i+60,2))
end 
```

we get excellent results. 

8. We consider again Problem 3: find x such that 

$f(x) = \int_{0}^{x}e^{-t^{2}}dt - 0.5 = 0.$ 

Since a function evaluation is expensive (summation of the Taylor series) but the derivatives are cheap to compute, a higher order method is appropriate. Solve this equation with Newton’s method. 

## Solution:

```txt
% IntegralExp.m
% Solve \int_{0}^{x} e^{-t^2}dt - 0.5 = 0 with Newton 
```

```matlab
% use ff.m to compute Taylor series
format compact, format long
x=1; xa=2;
while abs(xa-x)>1e-10
    xa=x;
    y=ff(x)-0.5; ys=exp(-x^2);
    x=x-y/ys
end

>> IntegralExp
x =
    0.329062444950818
x =
    0.532365165339031
x =
    0.550852862865461
x =
    0.551039408434969
x =
    0.551039427609027
x =
    0.551039427609027 
```

9. Using Newton’s iteration, find a such that $\int _ { 0 } ^ { 1 } e ^ { a t } d t = 2 .$ 

Solution: 

We have 

$$
\int_ {0} ^ {1} e ^ {a t} d t = \left. \frac {1}{a} e ^ {a t} \right] _ {0} ^ {1} = \frac {1}{a} e ^ {a} - \frac {1}{a}
$$

Thus we are looking for the solution of the equation 

$$
f (a) = \frac {e ^ {a} - 1}{a} - 2 = 0
$$

We use Newton’s method and get a 1.2564312086. 

10. Consider the billiard-problem. Let the ball P be at position P (0.5, 0.5) and let Q move in small steps (say 0.1) from 1 to 1. Compute for each position the solutions using bisection. Count and plot the solutions and plot also the function billiard. make a pause before moving on the the next position of Q. 

Solution: 

```matlab
% MainBilliard.m
% Animation for the billiard problem
clear, clf, format compact
figure(1)    % to show the billiard table 
```

```matlab
figure(2)    % to plot the function billiard(x)
pause    % to separate the two figures
global px py a    % ball positions P=(px.py), Q=(a,0)

px=0.5; py=0.5;

for a=1:-0.1:-1    % move Q
    a
    figure(1), clf(1)
    axis equal, hold
    t=0:0.01:2*pi;    % plot circle
    plot(cos(t),sin(t))
    plot(px,py,'o')    % plot point P
    text(px,py,'    P')
    plot(a,0,'o')    % plot point Q
    text(a,0,'    Q')
    P=[px,py]; Q=[a,0];

percent###
N=200; h=2*pi/N;    % sample billiard
xa=0; fa=billiard(xa);
k=0; Sols=[];
for i=1:N,
    xb=i*h; fb=billiard(xb);
    if fa*fb <=0;    % if sign change call Bisection
    x=Bisection(@billiard,xa,xb)    % compute angle
    k=k+1; Sols=[Sols,x];    % count and store solution
    X=[cos(x),sin(x)]    % Reflection point
    text(X(1),X(2),['    X',num2str(k)]);
    plot([Q(1),X(1)], [Q(2),X(2)])  % plot trajectory
    plot([X(1),P(1)], [X(2),P(2)])
    end;
    xa=xb; fa=fb;
end;

percent###
F=[];
X=0:0.01:2*pi;
for x=X
    F=[F,billiard(x)];
end

figure(2)
plot(X,F,[0,2*pi],[0,0])
legend('billiard(x)')
Sols
k
if a==1, pause    % to explain what is going on
else
    pause(1)
end

end 
```

11. Modify the fractal program by replacing $f ( z ) = z ^ { 3 } - 1$ with the function 

$$
f (z) = z ^ {5} - 1.
$$

(a) Compute the 5 zeros of f using the command roots. 

(b) In order two distinguish the 5 different numbers, study the imaginary parts of the 5 zeros. Invent a transformation such that the zeros are replaced by 5 different positive integer numbers. 

Solution: We first compute the zeros o $z ^ { 5 } - 1$ . The coefficients ofthe polynomial z<sup>5</sup> 1 are 

```txt
p=[1 0 0 0 0 -1] 
```

With the function roots we can compute the zeros 

```txt
>> W=roots(p)
W =
-0.809016994374948 + 0.587785252292473i
-0.809016994374948 - 0.587785252292473i
0.309016994374947 + 0.951056516295152i
0.309016994374947 - 0.951056516295152i
1.000000000000000 + 0.000000000000000i 
```

If we multiply the imaginary part by 2 we get 

```csv
>> 2*imag(W)
ans =
1.175570504584946
-1.175570504584946
1.902113032590305
-1.902113032590305
0 
```

Now we can add 3 and round the result to get 

```txt
>> round(2*imag(W)+3)
ans =
4
2
5
1
3 
```

By multiplying with the factor a 10 we get a beautiful fractal. 

```matlab
n=1000; m=30;
x=-1:2/n:1;
[X,Y]=meshgrid(x,x);
Z=X+1i*Y; % define grid for picture
for i=1:m % perform m iterations in parallel
    Z=Z-(Z.^5-1)./(5*Z.^4); % for all million points
end; % each element of Z contains one root 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/3a2e1d8344a09c125bd38f3ef51300aa60e971a89fda98a35b076c97760a9817.jpg)


## 12. Mandelbrot set: Consider the iteration

$$
Z _ {k + 1} = Z _ {k} ^ {2} + C.
$$

Depending on the value of the constant C the sequence $\{ Z _ { k } \}$ will either diverge to or converge. 

Let C now be in the region in the complex plane Z X iY with $- 2 \leq X$ , Y $\leq 2 .$ 

Perform 50 iterations starting always with $Z _ { 0 } = 0$ with all numbers C in that region and plot using image the resulting Mandelbrot set, which is the set of all values C for which the iterations converges to a finite limit. 

Solution: 

```matlab
% Mandelbrot.m
clf;
n=1000; m=50;
x=-1.6:2/n:1.6;
[X,Y]=meshgrid(x,x);
C=X+1i*Y; % define grid for picture
Z=0*C;
for i=1:m % perform m iterations in parallel
    Z=Z.^2+C; % for all million points
end; % each element of Z contains the limit
a=30;
image(isfinite(Z)*a); % and display image 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/49738e1503edafeb355bcffb7c699367a409b646e566658065d718e57ed0aac3.jpg)


## 10.9 Chapter 9: Simulation

1. Waiting for the elevator. We consider a building with n floors. A elevator is serving these floors and we are interested to know the distribution of the waiting time from pressing the elevator button till the elevator opens the door. 

Assume the time unit for the moving of the elevator one floor is one. We make m experiments in which the elevator is randomly located on one floor and the person is also coming randomly on one floor. The difference of the two floors is proportional to the time the elevator needs to come. 

Perform m 10,000 experiments for a n 10 floors building. Construct and plot the histogram of the waiting times. What is the most likely waiting time? 

Solution: 

```matlab
% Waiting for the elevator
clear, clf, clc
m=10000 % number of persons
n=10 % number of floors
A=zeros(1,n+1);
for j=1:m
    LocationElevator=round(rand*n);
    LocationPerson=round(rand*n);
    waiting=abs(LocationElevator-LocationPerson);
    A(waiting+1)=A(waiting+1)+1;
end
bar(A/m) 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/58712c53e44593410429cfee5665a478b52ae078d7ce852d6b352595d989216c.jpg)


It seems that most likely the elevator is one floor up or down when a person wants to use it. 

2. Given a set of points in the unit square. Write a program which computes and plots the two closest points. 

(a) Write a function [P,Q,minimum]=ClosestPoints(x,y) which computes all the distances between two points and stores the minimal distance and the two points P and Q which are closest. 

(b) Generate n points (x , y ) using the function rand. Then call the function ClosestPoints, plot the points and mark the two closest points by coloring them differently. 

## Solution:

```matlab
function [P,Q,minimum]=ClosestPoints(x,y)
% CLOSESTPOINTS computes the two closest point
%
n=length(x);
minimum=Inf;
for k=1:n
    for p=k+1:n
    dist=norm([x(k)-x(p);y(k)-y(p)]);
    if dist<minimum
    minimum=dist;
    kmin=k; pmin=p;
    end
    end
end
P=[x(kmin);y(kmin)];
Q=[x(pmin);y(pmin)];
for n = 20 we get for instance 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/29d3a9ceb04b2f39b73e276a579d03a8ceeaebf59d13602a38f8a1a40ec4458e.jpg)


## 3. Shortest distance between two point sets:

(a) Consider the circle with center (5, 6) and radius r 2 and the ellipse with center at origin and a 1 and b 0.5 parallel to the coordinate axis. Sample points on the ellipse and on the circle. Compute by brute force a point P on the circle and a point Q on the ellipse with minimal distance. Solution: 

```matlab
% DistEllipseCircle.m
% distance between a circle and an ellipse
clear, clf
t=linspace(0,2*pi,300);
X=[5+2*cos(t); 6+2*sin(t)]; % define circle
Y=[cos(t);0.5*sin(t)]; % define ellipse
axis([-2,10,-2,10])
axis square
hold
plot(X(1,:),X(2,:))
plot(Y(1,:),Y(2,:))
minimum=Inf; % compute points with
for x=X % minimal distance
    for y=Y
    dist=norm(x-y);
    if dist<minimum
    minimum=dist;
    P=x;Q=y;
    end
    end
end
plot([P(1),Q(1)], [P(2),Q(2)], 'or')
plot([P(1),Q(1)], [P(2),Q(2)], 'r')
distance=minimum
P,Q

>> DistEllipseCircle 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/faa286117112e1a4ce70ea34e647d6e92beec0b9f87ab6f5a6fef3abbeefd50d.jpg)


(b) The circle with center (5, 6) and radius r 2 and the ellipse with center (4, 4), a 2 and b 3 intersect. Try to compute the intersection points by brute force. Solution: 

```matlab
% IntersectEllipseCircle.m
% intersection points between a circle and an ellipse
clear, clf
t=linspace(0,2*pi,300);
X=[5+2*cos(t); 6+2*sin(t)]; % define circle
Y=[4+2*cos(t);4*3*sin(t)]; % define ellipse

axis([-2,10,-2,10])
axis square
hold
plot(X(1,:),X(2,:))
plot(Y(1,:),Y(2,:))

minimum=Inf; % compute points with
for x=X % minimal distance
    for y=Y
    dist=norm(x-y); 
```

```matlab
if dist<0.07 % 0.07 is by experiment
    dist
    P=x;Q=y; [x,y]
    plot([P(1),Q(1)], [P(2),Q(2)], 'or')
    end
    end
end

>> IntersectEllipseCircle
Current plot held
dist =
    0.0686
ans =
    5.5295 5.5109
    7.9286 7.8627
dist =
    0.0304
ans =
    5.8447 5.8737
    4.1871 4.1963
dist =
    0.0127
ans =
    5.8826 5.8737
    4.2053 4.1963
dist =
    0.0542
ans =
    5.9201 5.8737
    4.2242 4.1963 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/e37112840059ebf6e11ca63ba1888a4b8d3e50f5a7258cc69535995efda01071.jpg)



We obtain 3 times the approximations for the second intersection point.


4. Knapsack Problem: given a bag with a given maximum load limit W. Put in that bag items from the following table in order to maximize the sum of the value of the items but not exceeding the total weight W: 

<table><tr><td>item</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td></tr><tr><td>weights</td><td>3.3</td><td>4.6</td><td>1.7</td><td>5.8</td><td>7.7</td><td>3.1</td><td>5.3</td></tr><tr><td>values</td><td>7</td><td>9</td><td>5</td><td>12</td><td>14</td><td>6</td><td>12</td></tr></table>

Write a brute force program that solves the problem for a collections of bags: 

W 8, 10, 11, 15, 20, 21, 25, 26, 30, 32 

## Solution:

```matlab
% knapsack problem solved by brute force
clear, clf, clc

A=[1 2 3 4 5 6 7 % item number
    3.3 4.6 1.7 5.8 7.7 3.1 5.3 % weights
    7 9 5 12 14 6 12]; % values
BagSizes=[8,10,11, 15,20,21,25,26,30,32];

Values=[]; Weights=[];
P=perms(1:length(A));
[m,n]=size(P);
for W=BagSizes
    maximum=0;
    for k=1:m
    t=0; jj=n; % inspect row k
    for j=1:n % compute weights
    s=t; % not exceeding W
    t=s+A(2,P(k,j));
    if t>W
    jj=j-1; break
    end
    end
    s=0;
    for j=1:jj
    s=s+A(3,P(k,j)); % compute value
    end % and compare if larger
    if s>maximum % than current maximum
    maximum=s; row=k; col=jj;
    end
end
Sol=A(:,P(row,1:col))
weight=sum(A(2,P(row,1:col)))
value=sum(A(3,P(row,1:col)))
Weights=[Weights, weight];
Values=[Values, value];
W 
```

```txt
pause
end

plot(BagSizes, [Weights; Values], 'o')
hold
plot(BagSizes, BagSizes) 
```

We get the figure below where we see that the larger bags are the more also the total value increases. Furthermore the total weight remains always below the capacity of the bag indicated by the solid line. 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/4772bd2d3e7db67df0e808fd5aa29cd24c5f3c8c17157f9071ccd5cd22c039b9.jpg)


5. A dog would like to cross a river of width b. He starts at point $( b , 0 )$ with the goal to swim to (0, 0) where he has detected a sausage. His swim velocity $v _ { D }$ is constant and his nose points always to the sausage. The river flows north in direction of the y-axis and velocity of the flow of the river $v _ { R }$ is everywhere constant. 

(a) Develop the differential equation describing the orbit ${ \boldsymbol { z } } ( t ) = ( { \boldsymbol { x } } ( t ) , { \boldsymbol { y } } ( t ) ) ^ { \top }$ of the dog. 

(b) Program a Matlab function $\scriptstyle \mathtt { z p = d o g ( t , z ) }$ which describes the differential equation. The velocities $v _ { D }$ and $v _ { R }$ may be declared as global variables. 

(c) Use the program quiver and plot the slope field for $b = 1 , v _ { R } = 1$ and the following three cases for the dog velocity $v _ { D } = 0 . 8 , 1 . 0 \mathrm { a n d } 1 . 5 .$ 

Note: quiver $( { \tt X } , { \tt Y } , { \tt X } { \tt p } , { \tt Y } { \tt p } )$ needs 4 matrices. X and Y contain the coordinates of the points and Xp and Yp the two components of the velocity at that point. To compute these you can use the function dog e.g. 

$z=\text{dog}(0, [X(k,j), Y(k,j)])$ ; $Xp(k,j)=z(1)$ ; $Yp(k,j)=z(2)$ ; 

(d) Develop a Matlab integrator for the method of Heun of order 2 which integrates a given system of differential equations $\mathbf { y } ^ { \prime } = f ( t , \mathbf { y } )$ and stores the results in the matrix Z.The ith row of the matrix Z contains the values 

```matlab
function Z= OdeHeun(f,z0,tend,n)
% ODEHEUN integrates y'=f(t,y), y(0)=z0 with Heun from
% t=0 to tend using a fixed step size h=tend/n 
```

$$
[ t _ {i}, y _ {1} (t _ {i}), \dots , y _ {n} (t _ {i}) ].
$$

Compute and plot the orbits for the three dog velocities. You may want to stop the integration before executing all n steps when the dog arrives close to the origin or in the case when $v _ { D } < v _ { R }$ the dog is near the y-axis. 

## Solution:

(a) Let $ { \boldsymbol { z } } ( t ) = (  { \boldsymbol { { x } } } ( t ) ,  { \boldsymbol { y } } ( t ) ) ^ { \top }$ denote the position of the dog. The direction of the velocity vector of the dog points always to the the sausage at the origin. The velocity is overloaded with the river flow velocity which points north. Thus we get the system of differential equations: 

$$
\begin{array}{c} z ^ {\prime} (t) = \binom {x ^ {\prime} (t)} {y ^ {\prime} (t)} = - \frac {v _ {D}}{\sqrt {x (t) ^ {2} + y (t) ^ {2}}} \binom {x (t)} {y (t)} + \binom {0} {v _ {R}} \\ = - v _ {D} \frac {z (t)}{\| z (t) \|} + \binom {0} {v _ {R}} \end{array}
$$

(b) The Matlab function becomes 

```matlab
function zp=dog(t,z)
% dog, river problem
global vD vR
    zp=-vD*z/norm(z)+[0,vR];
end 
```

(c) The program for the slope field is 

```matlab
% Velocity field of RiverDog C.m
clear, clf
global vD vR
vR=1; vD=1.5;
r=(0:.06:1)
[X,Y]=meshgrid(r,r)
[m,n]=size(X);
Xp=zeros(m,n); Yp=zeros(m,n);
for k=1:m
    for j=1:n
    z=dog(0,[X(k,j),Y(k,j)]);
    Xp(k,j)=z(1);
    Yp(k,j)=z(2);
    end
end
quiver(X,Y,Xp,Yp) 
```

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/8a3226cc0f8f58fe4bb9453f76472dd9259c136a167d92e90e20c9d73785390e.jpg)


## (d) The Heun integrator becomes

```matlab
function Z= OdeHeun(f,z0,tend,n)
% ODEHEUN integrates y'=f(t,y), y(0)=z0 with Heun from
%    t=0 to tend using a fixed step size h=tend/n
global vR vD
y=z0; t=0; Z=[t,y];
h=tend/n;
for k=1:n
    k1=f(t,y); ys=y+h*k1;
    k2=f(t+h,ys);
    y=y+h/2*(k1+k2);
    t=t+h;
    Z=[Z; t y];
    if norm(y)<0.02 | (abs(y(1))<0.02 & vR>vD)
    break
    end
end 
```

we stop the integration when the dog is near the y axis or near the origin. The main program is 

```matlab
% RiverDog.m
clear, clf
global vD vR
vR=1;
%vD=0.8
vD=1
%vD=1.5
axis([-0.1,1,-0.1,1])
axis equal
hold on
z0=[1,0];
Z=OdeHeun(@dog,z0,10,500);
plot(Z(:,2),Z(:,3)) 
```

and the results for some dog velocities VD are 

![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/494db3e6a314dc06cc185b6604fe116d2d12f2dbddbd149679531c51d70f040c.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/6a4484a6f87beaaf477730ef264846ed13cf350022501e075790031df4f7e7f4.jpg)


![image](https://cdn-mineru.openxlab.org.cn/result/2026-11-17/a72b88da-1594-4496-b35a-24a18b1475e1/f7637a7461d45defca040d81280f359d8e6fbc363b277ea30a0ed53918168069.jpg)




1. Anderson, E., Bai, Z., Bischof, C., Demmel, J., Dongarra, J., Du Croz, J., Greenbaum, A., Hammarling, S., McKenney, A., Ostrouchov, S., Sorensen, D.: LAPACK Users Guide—Release 2.0. SIAM, Philadelphia (1992) 





2. Dongarra, J.J., Bunch, J.R., Moler, C.B., Stewart, G.W.: LINPACK Users’ Guide. SIAM, Philadelphia (1979) 





3. Gander, W., Gander, M.J., Kwok, F.: Scientific Computing Using Maple and Matlab. Springer, Heidelberg (2014) 





4. Gander, W., Hˇrebíˇcek, J.: Solving Problems in Scientific Computing Using Maple and Matlab, 4th edn. Springer, Heidelberg (2004) 





5. Garbow, B.S., Boyle, J.M., Dongarra, J.J., Moler, C.B.: Matrix Eigensystem Routines EISPACK Guide Extension. Lecture Notes in Computer Science. Springer, Berlin (1977) 





6. Grau, A.A., Hill, U., Langmaack, H.: Translation of ALGOL 60. Springer, Berlin (1967) 





7. Moler, C.B.: MATLAB Users Guide. Report. University of New Mexico, USA (1980) 





8. Moler, C.B.: Experiments with matlab, on line tutorial. http://www.mathworks.com/moler/ exm/chapters.html (2011) 





9. Quarteroni, A., Saleri, F., Gervasio, P.: Scientific Computing with MATLAB and Octave. Springer, Berlin (2014) 





10. Rutishauser, H.: Description of ALGOL 60. Springer, Berlin (1967) 





11. Smith, B.T., Boyle, J.M., Dongarra, J.J., Garbow, B.S., Ikebe, Y., Klema, V.C., Moler, C.B.: Matrix Eigensystem Routines—EISPACK Guide. Lecture Notes in Computer Science. Springer, Berlin (1976) 





12. Wilkinson, J., Reinsch, C.: Linear Algebra. Springer, Berlin (1971) 





13. Wirth, N.: Algorithms and Data Structures. Prentice Hall, New Jersey (1986) 

