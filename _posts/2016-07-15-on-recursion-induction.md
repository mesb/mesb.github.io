---
layout: post
title: On Recursion, Recurrences, Induction and Mathematical Sciences
publish: true
---

# On Recursion, Recurrences, Induction and Mathematical Sciences<a id="orgheadline2"></a>

Very often I wake up thinking I&rsquo;ve understood the concept of recursion, but I am
always struck by a feeling of abondonment when I try to capture my thoughts
on the topic. &ldquo;Not today&rdquo; was my response to that feeling this time around. In
these notes, I intend to capture plausible and reasonable literature on
recursion and its neighboring concepts, recurrences and induction.

The mind is a great tool, and it is often impossible to separate certain
sciences from the capabilities of the mind. I remember having a philosophical
discussion about the origins of mathematics. We were asked &ldquo;Was Mathematics
invented or created?&rdquo; I thought deeply about this question and what my shallow
mind reluctantly settled on about this question was another question. So I
described the following situation:
Imagine a scene about the first men to live. How did one man or woman entertain
the idea that he/she had 2 hands or 2 legs or 2 eyes? Perhaps, they never used
the word &ldquo;two&rdquo;, but to some degree they understood the idea of &ldquo;twoness&rdquo;.
Similarly, when they went hunting, how did they separate 1 deer from 2? An infinitude
of questions like these can arise, but I&rsquo;ll stop here for now.

To be brief, mathematics is a feature of our minds. The science of mathematics
is a frame we use to express that mathematical nature of our own minds. So in
some sense, mathematics was not created and in the same sense and others, the
science of mathematics was invented. Interestingly, a box of fine tools come
along with mathematics, useful, evident, strong and like some would say
beautiful. One of those tools is the concept of induction, or to be more precise
mathematical induction as opposed to empirical induction.

Jules Henri Poincaré and a host of others expressed the following about
mathematical induction: &ldquo;If a theorem is true for the number 1, and if it has
been proved that it is true for *n+1* provided it is true for *n*, it will be true
of all positive whole numbers.&rdquo; These lines capture the essence of mathematical
induction, but an example is necessary to actualize its essence with an
observation of the addition of whole numbers. We may have heard jokes about
mathematicians and their abilities to conjure assumptions. So we will follow
their lead.

Assume that the operation *x + 1* has been defined, and it expresses the idea of
adding *1* to a number *x*. That is all we need to know. Consequently, the operation
*x + a* expresses the idea of adding the number *a* to a given number *x*. Also,
presume that the operation *x + (a - 1)*, therefore

*x + a = [x + (a - 1)] + 1* -----&#x2013;&#x2014; (1)

That is adding *a* to a number *x* is thesame as adding one to the number that
precedes *x+a*. Hence, we know *x+a* when we know *x+(a-1)*, and *x+1*
gives birth to *x+2*, *x+3*, etc. Let&rsquo;s entertain a subtle demonstration for a
bit. Remember *x+1*? From it we get:

-   *1 + 1 = 2*
-   *2 + 1 = 3*
-   *3 + 1 = 4*

In the same light, we can define *x + 2* as *x + 2 = (x+1) + 1*

In a mathematical sense, the operation *x+1* is called a **recurrence**. We shall
come to understand that a recurrence is analogous to a device, an abstract
device in this case, constructed to embody an experiment so that an infinitude
of test objects could be experimented upon to conceive and maybe confirm the
validity of a hypothesis or truth.

With addition defined, let us investigate the validity of one of its laws: the
associative law of addition.

**a + (b + c) = (a + b) + c;** --------------&#x2013;&#x2014; (\*)

Let *c = 1*, then
        *a + (b + 1) = (a + b) + 1*  --------------&#x2013;&#x2014; (2)

The notes above will confirm that (2) above is an example of equation
(1). Since by addition we are taught the idea that predecessors imply successors
and successors imply the existence of predecessors, let us assume that the
associative law is true for *c = w*, in the light of the predecessor-successor
law it will be true for *c = w + 1*.

Let *(a + b) + w = a + (b + w)*;

It follows that

*[(a + b) + w] + 1 = [a + (b + w)] + 1;*

also evident from definition (1). And

*(a + b) + (w + 1) = a + (b + w + 1) = a + [b + (w + 1)];*

which establishes that truth of the law for *w + 1*. Hence, the law is true for
*c = 1*, true for *c = 2*, *c = 3* etc.

As a recap, this series of reasonings have enabled us to confirm a mathematical
law without enduring the hassles of monotously testing all the whole numbers,
that is an infinite number of test cases. In fact, we did not test up to a hand full of numbers. All we did was to show that
the law is true for *n = 1*, then we showed that if it is true for *n-1* it is
true for *n*, and eventually we concluded that it is true for all whole numbers.
And as you know there are an infinite number of whole numbers, but here we are
able to chase infinity and prove a law true.

This tiny art of proving a theorem or law for such huge sets and using the steps
we used above is called *proof by recurrence*. Poincare had this to say about
proof by recurrence a.k.a proof by induction:

*The essential characteristic of reasoning by recurrence is that it
contains, condensed, so to speak, in a single formula, an infinite number of
syllogisms.*

To contrast this approach with that of the physicial sciences, we observe a
similar flow of the monotony of the experiments, but a little further into the
experiments we are slapped by the monotony of the exercise and we face the truth
all physical sciences profess: &ldquo;we can only approximate truth, we can not be
absolutely certain.&rdquo; An assault on this statement endows us with the idea that
since we cannot conduct physical experiments for every possible physical use
case, we can only approximate the truth about physical laws.

As is evident by now, by induction, we construct test subjects for our
mathematical experiments, and by recurrences, we construct the necessary and
very robust, so to speak, experimental devices. Armed with these tools and
understanding we can face the concept of recursion.

So the question becomes *what is recursion?*

Before looking into that, let&rsquo;s enunciate the parts of recurrences and
induction. A recurrence is an experimental device that receives input and
returns output. Induction is a mathematical tool that generates an infinite
amount of test cases, at least in the domain of whole numbers, that are fed to
recurrences for experimentation. Induction has a precise and definite starting
point, something like *n = 1* and has no end. It allows us to pursue infinite
cases.

Induction and recursion have thing in common, and that is *recurrences*.
Induction is a bottom-up construction process, most often from *n = 1*  to
infinity. A recurrence as described by Poincaré enables us to use the same
device on an infinite set of test cases. Hence, recursion and induction differ
only in orientation. And by orientation, I mean where they start and how to
propagate to their end from the start.

In computer science, recursion is often defined as the tecnhique where a
procedure invokes itself on smaller instances of the same problem, provided the
smaller instances of the problem are homogenous to the original problem. At face
value, we may divorce the recurrence device from the concept of recursion, but
as mentioned above recursion is only a situational view and use of a recurrence
device. A recurrence can be seen as a harsh task master in need of a pilot to
specify its start and end values, and this is where recursion and induction come to play.

Therefore, in recursion, we specify a recurrence, we determine the start and end
values of our experiment or procedure, and we feed the values to our recurrence.
Below is an example to drive home the idea of recursion.

Suppose we want to construct a power function. That is a function of the form:

*f : a x b &#x2014;> c*

*a ^ b = c*

This function expresses the idea of multiplying a quantity *a* by itself *b*
times. Immediately it becomes evident that a muiltpying device will serve as our
recurrence. And by recursion, we can put this recurrence to use, specifying *a*
and *b* accordingly to obtain *c*.

Let&rsquo;s contruct our recurrence. For multiplication, we begin with the
commutatinve law:

*a x 1* = *1 x a;*   -------&#x2013;&#x2014; (3)

It will be fun to investigate and prove this law, but I&rsquo;ll leave that out for
now. We have obtained the starting point, or most primitive form of our
recurrence. This is often given the name **base case**. The base case is also
called the **base case** in inductive investivations, and is usually *n = 1*.

The recurrence equation can do the following:

multiply *a* by *a ^ (b-1)* times.

*a ^ b = a x [ a ^ (b -1) ]**

But the operation (b - 1) can go on forever. When do we stop? This question can be answered by
(3) above. We stop when *b = 1*. Interestingly, this thinking leads us to a
use case problem. What happends of we receive a task to compute *b ^ 0)*? Well,
interestingly, the power function is itself a machine or procedure with its own
rules, which uses as a mechanism the multiplication procedure. According to the
laws of power functions,

*a ^ 0 = 1*

*a ^ 0 = 1* -----------&#x2013;&#x2014; (4)

Generalized as *a number to the power zero is 1*. There are special exceptions to
this statement, which we shall skip for now.

Armed with insight for computing powers, we can construct our recurrence
device using multiplication and the statement in (4) above.

*a ^ b = a x [a ^ (b -1)] if **b >= 1**, and 1 if b = 0.*  --------&#x2013;&#x2014; (5)

It must also be mentioned that b must be greater than or equal to 0.

So our recursion works by reducing itself towards the base case and perculating
the values arrived at on the base and its successors back through a series of deferred operations.

Let us make this implementation concrete by expressing it in a programming
language called scheme.

    ;; pow: a x b ----> c
    ;; usage: (pow a b) ----> Int
    (define pow
        (lambda (a, b)
            (if (= b 0) 1
                (a * (pow a (- b 1))))))

    ;; (pow 2 3) ---> 8

**Recurrence**: pow

By recursion we supply *a* and *b* to the recurrence **pow** to obtain the result
*c*

## References<a id="orgheadline1"></a>

1.  Foundations of Science by Jules Henri Poincaré
