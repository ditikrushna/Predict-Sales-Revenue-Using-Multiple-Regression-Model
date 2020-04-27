Data Science Math Skills
========================

Maths is the language of Data Science.

Week 1
======
Building Blocks for Problem Solving

a. Sets and What they're good for
+++++++++++++++++++++++++++++++++

Sets basics and vocabulary:
--------------------------

A Set is a collection of things.
A Set is made up of elements.

A = {1, 2, -8}

Notation:
2 ∈ A (2 belongs to A)
8 ∉ A (8 doesn't belongs to A)

Cardinality:
Size of a set A is the number of elements in A.
∣A∣ = 3

A = {1, 2, -3, 7}
B = {2, 8, -3, 10}
C = {5, 10}

A ∩ B (A Intersection B) = {2, -3}
A ∪ B (A Union B) = {1, 2, -3, 7, 8, 10}
A ∩ C = ∅ (Empty set)

In general:
A ∩ B = {x: x ∈ A and x ∈ B}
A ∪ B = {x: x ∈ A or x ∈ B}

Sets: Medical Testing Example:
-----------------------------

VBS: Very Bad Syndrome
X = set of people in a clinical trial

S = {x ∈ X: x has VBS}
H = {x ∈ X: x does not have VBS}

S ∪ H = X
S ∩ H = ∅

P = {x ∈ X ∣ x test positive for VBS}
N = {x ∈ X ∣ x test negative for VBS}

P ∪ N = X
P ∩ N = ∅

S ∩ P = True Positive
H ∩ N = True Negative
S ∩ N = False Negative
H ∩ P = False Positive

∣S∣ / ∣X∣ = Proportion of people in study having VBS

∣H∣ / ∣X∣ = Proportion of people in study without VBS

∣S ∩ P∣ / ∣S∣ = True Positive Rate

∣H ∩ P∣ / ∣H∣ = False Positive Rate

|S ∩ N∣ / ∣S∣ = False Negative Rate

∣H ∩ P∣ / ∣H∣ = False Positive Rate

Sets: Venn Diagrams:
--------------------

Visualizing Sets

Inclusion-Exclusion Formula:
∣A ∪ B∣ = ∣A∣ + ∣B∣ - ∣A ∩ B∣

b. The infinite world of real numbers
+++++++++++++++++++++++++++++++++++++

Numbers: The Real Number Line
-----------------------------
Natural Numbers
Whole Numbers
Integers
Rational Numbers
Irrational Numbers
Real Numbers

Positive Reals
Negative Reals

Absolute Value of a real number X, |X| is the distance from X to 0.

In general rule:
For any x ∈ R
∣X∣ = { x if x is non-negative
		-x if x is negative }

Numbers: Less-than and Greater-than
-----------------------------------
a < b (a is less than b)
a > b (a is greater than b)
a <= b (a is less than or equal to b)
a >= b (a is greater than or equal to b)
a << b (a is much much less than b)

Numbers: Algebra with Inequalities
----------------------------------
Rules:
if a = b, then a + c = b + c
if a = b, then a * c = b * c
if a < b, then a + c < b + c
if a < b, then a * c < b * c if c is postive number otherwise a * c > b * c

Numbers: Intervals and Intervals Notation
-----------------------------------------

Closed Interval:
[2, 3.1] = {x ∈ R: 2 <= x <= 3.1}

Open Interval:
(5, 8) = {x ∈ R: 5 < x < 8}

Half Open Interval:
[1, 10) = {x ∈ R: 1 <= x < 10}

c. That Jagged S Symbol
+++++++++++++++++++++++

Sigma Notation: Introduction to Summation
-----------------------------------------
Σ (Sigma)

Sigma notiation comes with start and end range along with dummy indices in the 
	notation.

Σ (i = 1 to 4) (i^2) = 1^2 + 2^2 + 3^2 + 4^2 = 30

Sigma Notation: Simplication Rules
----------------------------------
Σ (Ki) = K Σ (i) where K is constant

Distributive Property: A(b + c) = Ab + Ac

Σ (i^2 + 2i) = Σ (i^2) + Σ (2i) = Σ (i^2) + 2 Σ (i)

Σ (K) != K but it is Σ (K i^0) = K * range

Sigma Notation: Mean and Variance
---------------------------------
X = {x1 x2 ... xn}

Mean (Mu) = 1/n Σ xi

Mean Centering:
Removing mean from each element, making the mean of the elements to be zero.

Variance: (How spread out the data set)
Variance = 1/n Σ (xi - Mean)^2

For e.g
Z = {1, 5, 12} & W = {5, 6, 7}
Mean (Z) = 6
Mean (W) = 6
Variance (Z) = 62/3
Variance (W) = 2/3

Standard Deviation = sqrt(variance)

--------------------------------------------------------------------------------

Week 2
======
Functions and Graphs

a. Descartes was really smart
++++++++++++++++++++++++++++++

Cartesian Plane: Plotting Points
-------------------------------
|R^2 (x, y) axis

Origin (0, 0)

X axis = {x, y ∈ |R^2: y = 0}
Y axis = {x, y ∈ |R^2: x = 0}

First Quadrant: {x, y ∈ |R^2: x > 0, y > 0}
Second Quadrant: {x, y ∈ |R^2: x < 0, y > 0}
Third Quadrant: {x, y ∈ |R^2: x < 0, y < 0}
Fourth Quadrant: {x, y ∈ |R^2: x > 0, y < 0}

Cartesian Plane: Distance Formula
---------------------------------
Pythogorean theorm: z^2 = x^2 + y^2

Distance Formula: (a, b) (c, d)
d = sqrt((c-a)^2 + (d-b)^2)

Nearest Neighbor is the least distance point from a point.

Clustering:
If A & B are in cluster X, C in cluster Y
Then Distance (A, B) << Distance (A, C) or Distance(B, C)

Cartesian Plane: Point Slope formula for lines Part 1
-----------------------------------------------------
A = (a, b) B = (c, d)

Slope (m) = (d-b) / (c-a) = Rise / Run

Slope is defined as if we move 1 unit in x axis, then in order to reach B
	from A, we move slope units in y axis.

Equation of line:
Suppose (2, 1) and (3, 2) forms a line
Slope = 1
1 = (y-1) / (x-2)
x - y = 1 is the equation of the line

Point Slope Formula:
If a line l has slope M and if (xo, yo) is any point on the line, then l has the
	equation
y - yo = M (x - xo)

Cartesian Plane: Point Slope formula for lines Part 2
-----------------------------------------------------
y intercept formula (0, b)
y = x - 1

If a line l has lope M and l hits the y axis at the point (0, b), then
	y = mx + b is the equation of the line

b. Input Output Machine
+++++++++++++++++++++++

Functions: Mapping from Sets to Sets
------------------------------------
A function f: A->B is a rule/formula/machine which transforms each a ∈ b into
	f(a) ∈ B

For e.g
X = {All people in VBS study}
y = {+, -}

Function test: X->y 
test(person) = +
test(person) = -

Supervised Learning:
Input(A) and Output(B) is given (Samples)
Find function f: A->B

Functions: Graphing in the Cartesian Plane
------------------------------------------
f: |R->|R
For e.g 
f(x) = 2x - 1

In general, if g: |R -> |R
the graph of g is graph(g) = {(x, y) ∈ |R^2: y = g(x)}

Vertical Line Test:
Any line of a graph will touch vertical axis only one time.

Functions: Increasing and Decreasing Functions
----------------------------------------------
Let f: |R -> |R
f is strictly increasing if whenever a < b, we have f(a) < f(b)
f is strictly decreasing if whenever a < b, we have f(a) > f(b)

Some functions f(x) = x^2 is neither strictly increasing nor decreasing.
But, these functions are strictly increasing or strictly decreasing in certain
	intervals.

Horizontal Line Test:
A function is strictly increasing or decreasing if it intersects horizontal line
	exactly once.

Functions: Composition and Inverse
----------------------------------
f(x) = x^2
g(x) = x + 5

gof(x) = g(f(x)) = x^2 + 5
fog(x) = f(g(x)) = (x+5)^2

gof(x) != fog(x)

For e.g
f(x) = 2x
g(x) = (1/2)x

gof(x) = g(f(x)) = x
fog(x) = f(g(x)) = x

Here, f and g are inverse of each other.

Not every function has an inverse function.
If a graph of f fails the horizontal line test, then f has no inverse.

--------------------------------------------------------------------------------

Week 3
======
Measuring rates of change

a. This is about the derivative stuff
+++++++++++++++++++++++++++++++++++++

Tangent Lines: The Slope of a graph at a point
----------------------------------------------
Tangent Line to graph of f(x) at x = A
Its slope gives rate of change of f(x) at x = A

f'(a) is the derivative of a function f(x) at x = A

f'(a) = lim h->0 (f(a + h) - f(a)) / h

Tangent Lines: The Derivative Function
--------------------------------------
f(x) = x^2

f'(x) = lim h->0 ((x + h)^2 - x^2) / h
	  = lim h->0 ((x^2 + h^2 + 2xh) - x^2) / h
	  = lim h->0 h(2x + h) / h
	  = lim h->0 (2x + h)
	  = 2x

b. Fast Growth - Slow Growth
++++++++++++++++++++++++++++

Using Integer Exponents
-----------------------
Positive Integer Exponents:
9 = 3^2 (3 Square)
27 = 3^3 (3 Cube)

Zero as exponent:
3^0 = 1

Negative Integer Exponents:
2^-1 = 1/(2^1)
2^-2 = 1/(2^2) = 1/4

Scientific Notation:
5.9 x 10^24
9.1 x 10^-31

Simplication Rules for Algebra using Exponents
----------------------------------------------
a. Multiplication Rule
x^n x^m = x^(n+m)

b. Power to Power Rule
(x^n)^m = x^(n*m)

c. Product to Power Rule
(xy)^n = x^n y^n

d. Fraction to a Power Rule
(x/y)^n = x^n/y^n

e. Division and Negative Powers
x^n/x^m = x^(n-m)

Fractional Exponents:
x^(a/b) = b root of x^a

How Logarithms and Exponents are related
----------------------------------------
b^x = N
x = logb(N)

Logs of any base 1 = 0

a. Product Rule
log(xy) = log(x) + log(y)

b. Quotient Rule
log(x/y) = log(x) - log(y)

c. Power & Root Rule
log(x^h) = h(log(x))

The Change of Base Formula
--------------------------
log2(12) = 3.585
log10(12) = 1.079

loga(b) = logx(b) / logx(a)

The Rate of Growth of Continuous Processes
------------------------------------------
Discrete exponential rate of growth
Continuous exponential rate of growth (e)

e = 2.71828

ln(x) = natural log = log to the base e

--------------------------------------------------------------------------------

Week 4
======
Introduction to Probability Theory

a. Basic Probability Definitions
++++++++++++++++++++++++++++++++

Probability Definitions & Notations
-----------------------------------
Certainty at which statement is true.

P(x) + P(~x) = 1

Probability Distribution: All the probability sums upto 1.
Collection of statements which are exclusive and exhaustive forms the distribution.

P(event) = Number of outcomes defined as in event/Total # of outcomes in universe.

Joint Probabilities
-------------------
P(A and B)
P(A, B) = P(B, A)

Order doesn't matter.

Independent definition:
P(x, y) = P(x) P(y) (Product Distribution)

P(A or B) = P(A) + P(B) - P(A, B)

b. Problem Solving Methods
++++++++++++++++++++++++++

Permutations & Combinations
---------------------------
Permutations - Order Matters
Combinations - Order doesn't matter

Permutations: n!/(n-m)!
Combinations: n!/(n-m)!m! (n choose m)

With replacement & without replacement probability.

Using Factorial and "M choose N"
--------------------------------
With replacement experiement are independent experiments.

M choose N: 
Number of distinct groups of n items drawing from m items without replacement.

The Sum Rule, Conditional Probability, and the Product Rule
-----------------------------------------------------------
Probability of individual event = Sum of Joint Probabilities

P(A) = P(A, B) + P(A, ~B)
P(A) = P(A, B1) + P(A, B2) ... P(A, Bn)

Conditional Probability P(A|B)
What is probability of A given B is true.

= (Relevant Outcomes) / (Total outcomes in Universe when B is true)

Product Rule:
P(A|B) = P(A, B) / P(B)

If A & B is independence, then P(A|B) = P(A)

c. Applying Bayes Theorem and the binomial theorem
++++++++++++++++++++++++++++++++++++++++++++++++++

Bayes' Theorem (Part 1)
-----------------------
P(A|B) = P(B|A) P(A) / P(B)

It is used to get the probability of a process given the outcome.

Bayes' Theorem (Part 2)
-----------------------
it is also used to update the probability calculated before.

Posterior Probability = Likelihood * Prior Probability / Marginal Probability

The Binomial Theorem and the Bayes Theorem
------------------------------------------
n = number of independent trails
s = number of successes
p = probability of 1 success

(n choose s)(p^s)(1-p)^n-s
