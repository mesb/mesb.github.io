---
layout: post
title: growth of algorithms
publish: true
---

# Growth of Functions<a id="orgheadline11"></a>

Functions are incarnations of algorithms. As these functions evolve they consume
computational resources. Also, functions are often called procedures in
computations and the algorithm-function relationship gives birth to what is
called procedural abstraction. That is what ever procedure is harshed from a
function/algorithm is independent in its own right and solves the intended
problem in its own way. Several procedures with the same name could actually
implement different algorithms, but all arrive at the same solution. In this
case, each of the procedures is called a procedural abstracion.

An example is a square root function. THe square root of a number could be
calculated in a variety of ways:

1.  Newton&rsquo;s method or using a binomial expansion of power 1/2
2.  Using fixed points
3.  Using the Egyptian Method or starting with a guess and improving it&#x2026;

All these algorithms would arrive at the squareroot of a number, therefore we
have a choice. And if we have a choice, then we need to use a scale of
preference, and opportunity costs to determine which of the algorithms to use. A
closer look at the concept of scale of preference reveals that we might chose
the algorithm that uses less time to compute the result we are seeking. And the
opportunity cost will enable us get a feel of what we shall loose if we chose
one algorithm over the others. Eventually, we need a proper understanding of
the implications of using any algorithm we choose. How can we understand what
we loose or gain from an algorithm?

The procedures can be formally analyzed to understand the their comsumption of
resources. It is this formal understanding that will help us classify
algorithms, choose which is better in what situation, communicate our ideas
about algorithms, and be able to know what
and where to tweak performance.

The study or analysis of the run times of algorithms is investigated and
expressed formally using a notation called asymptotic notation. We could call
these investigations the Calculus of Algorithms or Algorithmic Calculus.

Note that differential and Integral Calculus are tools that can also be
implemented to get an understanding of the rates of change of various
Algorithms and also to compute the total amount of resources consumed by an
algorithm.

The time taken by an algorithm to perform each step, and eventually the total
time taken to return a result plus the sum total of the cost of every step
taken is called the running time of an Algorithm.

The running time is often expressed as a Mathematical function. Therefore, we
could apply differential calculus to the emergent runtimes functions of various
algorithms to determine their growth rates.

Similarly, the application of integral calculus as a tool for determining the
total run time, total cost, average cost, total space etc. of an algorithm is
very feasible.

Suppose there is loop that runs n times and uses x steps. The total cost of
such a loop can be determined by using the integral of x from 1 to n.

That is, c &times; &int;<sub>0</sub><sup>n</sup>  x dx = c &times; \textonehalf{} &times; n<sup>2</sup>

Where c is a constant.

## Asymptotic Notation<a id="orgheadline9"></a>

See the Mathematical concepts of Limits, Sequences and Series  for more understanding of the analysis
of the algorithms.

### Asymptotes<a id="orgheadline1"></a>

In Mathematics, an asymptote refers to a line or curve that approaches a given
curve arbitrarily closely, but never touches it. Vertical asymptotes arise when
dealing with rational functios such that the value of the denominator becomes
zero. Vertical asymptotes can tell us more about the domain of a function.

Horizontal asymptotes are values, curves or lines that anothe function
approaches very closly without actually reaching it. That is as the values of
the function grow large without bound, the value it approaches often tend to be
the Horizontal asymptotes. Same as the limit of a function as it approaches
infinity.

lim<sub>x &rarr; &infin;</sub> x = L

Interestingly, L could actually be a function. That is:

lim<sub>x &rarr; &infin;</sub> x = g(x)

### Asymptotic Notation<a id="orgheadline6"></a>

Now, in computer science, Asymptotic notations are used to express the rate at
with algorithms grow by expressing the functions that the runtimes of these
Algorithms approach as their inputs become large without bound.

Suppose f(n) is an Algorithm with input n, and suppose there is a set of some
other functions collectively called g(n). The asymptotic notation of the run
time of f will tell us how f approaches g as n becomes larger and larger, in
the same way that a normal mathematical function will evolve and approach it&rsquo;s
horizontal Asymptote.

1.  **&Theta; - notation**

    Used to express the growth of an algorithm A(n) relative to some other function F(n)such
    that given 3 constants c<sub>1</sub>, c<sub>2</sub>, n<sub>0</sub>, for all inputs n > n<sub>0</sub>, A(n) is &ge; c<sub>1</sub> &times; F(n) from
    below and &le; c2 &times;  F(n) from above. Therefore, A(n) is sandwiched between
    c<sub>1</sub> &times; F(n) and c<sub>2</sub> &times; F(n).
    
    Expressed as: 0 &le; c<sub>1</sub>F(n) &le; A(n) &le; c<sub>2</sub> F(n) for all n &le; n<sub>0</sub>
    
    However, when communicating such information, we often say:
    
    A(n) = &Theta;(F(n))
    
    Although we actually mean A(n) &isin; &Theta;(F(n))
    
    The sandwich or pinching theorem of limits justifies our notation.
    
    According to the squeeze or sandwich theorem of limits [<span class="underline">Squeeze Theorem</span>](https://en.wikipedia.org/wiki/Squeeze_theorem)
    From this, it is concluded that F(n) is an asymptotically tight bound for A(n).

2.  **O - notation**

    From &Theta;-notation, which has both upper and lower bound, it follows that
    there is a situation where there is either an upper bound or a lower bound and
    not both. A case with no lower bound, that is Asymptote tight bound minus the
    lower bound, is expressed using the O-notation. This is called an Asymptotic
    upper bound.
    
    Expressed as: 0 &le; A(n) &le; cF(n) for all n &ge; n<sub>0</sub>
    
    It might be compelling to realize that an Algorithm whose run time is &Theta;(n)
    is a subset of that whose run time is 0(n).
    
    That is,
    
    &Theta;(F(n)) \subseteq O(F(n))
    
    Often, when taking the run times of Algorithms we omit constants, leading
    coefficients, and take just the leading term. An notaion of F(n) = &Theta;(n<sup>2</sup>)
    might actually mean that F(n) = a n<sup>2</sup> + b n + c.
    
    The fact that
    
    &Theta;(n) \subseteq O(n),
    
     explains this elimitation of minor terms
    and the leading coefficient.
    
    Similarly, a algorithm with a growth rate of *a &times; n + b* is linear, but can
    be expressed as A(n) = &Theta;(n<sup>2</sup>)
    
    1.  Note
    
        The upper hints the worst case, which is what we are often interested in
        knowing. So O-notation tells us about without getting us engaged in sophistaced
        calculations.
        
        For example, the insertion sort Algorithm has 2 major loops. Loop one has a
        runtime of n, and loop 2 a run time of n, therefore the upper bound is n &times;
        n which is n<sup>2</sup>. And this is the actual run time of insertion sort Algorithm.
        
        In effect, all what run times express are the bounds of the consumption of
        resources and not the exact run times of every instance of the algorithm in question.

3.  **&Omega;-notation**

    And finally the lower bound. If there is a function F(n) such that for all n,
    an algorithm A(n) is &ge; F(n), then F(n) is a lower bound to that algorithm,
    A(n).
    
    Expressed as: 0 &le; cF(n) &le; A(n) for n &ge; n<sub>0</sub>

### Theorem<a id="orgheadline7"></a>

A function is bouned if and only if it is bounded from below and above.

For any 2 functions f(n) and g(n), we have f(n) = &Theta;(g(n)) if and only if
f(n) = O(g(n)) and f(n) = &Omega;(g(n))

Therefore, the run time of insertion sort is &Theta;(n) from below and
&Theta;(n<sup>2</sup>) from above.

### Opposite of Asymptotically tight bounds<a id="orgheadline8"></a>

In numberline arithmetic, &lt; is know as strictly less than. In Asymptotic
analysis, Asymptotes with &le; are called Asymptotically tight bounds. The
Opposite of this or bounds that are strictly less than or greater than are
expressed using little notations:

1.  little oh: o(g(n))
2.  little omega: &omega;(g(n))

## Mathematical functions and conepts<a id="orgheadline10"></a>

1.  Monotonicity
2.  Floors and Ceilings
3.  Modular Arithmetic : a &le; a mod n < n
4.  Polynomials: p(n) = \displaystyle&sum;<sub>i=0</sub><sup>n</sup> a<sub>i</sub>  n<sup>i</sup>