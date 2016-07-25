---
layout: post
title: Notes on SICP lecture 1, part 1
publish: true
---

# SICP Lecture 1 Part I<a id="orgheadline12"></a>

"Computer science is a terrible name for this business" are the magical words
Professor Hal begins the lecture with. The name computer science is an example of
confusion between the tools used in a science, for the science itself. Much in
the same way that geometry is not about the tools for measuring or surveying the
earth, and physics is not about particle accelerators.

In errecting geometry, the Egyptian priesthood were beginning to systematically
put in place rules and methods to determine and express what is true. Their mathematics
involved space and time and they set up axiomatic frameworks that could
establish the truthfullness or falsity of geometrical propositions. Eventually, they
revolutionarized mathematics.

Computer science is similar, but it is not about computers, and it is also not
a science. It is like magic. It involves formalizing the organization and
execution of &ldquo;how to&rdquo; knowledge. It is the systematic study of &ldquo;process&rdquo; or &ldquo;method&rdquo;.

It is formalizing intuitions about process. How to do things. Starting to
develope a way to talk precisely about &ldquo;how to&rdquo; knowledge.

It is different from mathematics which involves formalizing intuitions about &ldquo;what
is&rdquo; knowledge. Mathematics will declare what you are looking for, but not how
to get it.

Computer science will imperatively tell you how to get to what you are looking
for.

In computer science, procedures are used to direct processes. And then, you
will ask, what is the origin of a procedure? Procedures are composed using programming languages.

But then, we can&rsquo;t stop at composing procedures. As the systems or processes we
describe get larger, things get complex. So, we in computer science also have to
formalize the management of complexity. We want to be able organize things so
that we can understand them, and upgrade them seamlessly.

Computer science deals with idealized components.

The contraints imposed in building large systems are the limitations of our own
minds. Unlike physics or other physical sciences where some physical laws or phenomena
like heat or speed of light can impede our progress.

In computer science, we create abstractions of physical systems and represent
them as much as we want, as much as we can idealize them.

## Ways of managing complexity<a id="orgheadline8"></a>

### Blackbox abstraction<a id="orgheadline4"></a>

Design and construct machinery that can be used generally without having to
comprehend their inner mechanisms. It is like building a machine that can be used over and over
without actually looking into its parts. And importantly, the machine can be
used as a part in some other larger machine or system.

In our case, what enables us to embody a set of general rules for solving a
class of problems is our ability to abstract things. In so doing, we collect
all what can be solved by our method, while simultaneously separating it from
all other methods that are different from it. This is called abstraction.

Incidently, we use our language to construct these black boxes that will
perform computations for us. We use our language to build the parts of the
box, in the same way that a machinist will use metals to construct machines.

We use our language to describe the imperative knowledge of performing our
computation.

1.  Note

    Our ability describe or errect black boxes is not limited to 1 level. That is,
    we do not have to describe methods that return only values or the answers. We
    are very free to describe black boxes that will inturn return the desired
    abstractions that we need. In other words, we can describe procedures that will
    compute and spit out procedures that perform the required computations.

    Reasons for using procedures that return procedures is because procedures is our
    way to talk about imperative knowledge. And in cases were the talked about
    procedure is actually a means to another procedure, it will be just to return
    the required procedures from the procedures we started with.

2.  procedures.

3.  Example

    Imagine that you have a procedure that performs the &ldquo;AND&rdquo; boolean function on
    one bit. How do you scientifically create a similar proc for 8 or n bits.

    A simple solution is to create a procedure that takes the AND function, if
    needed, and returns a procedure that performs AND on 8 bits.

    So we should be able to talk about knowledge that talks about other knowledge.

### Conventional Interfaces<a id="orgheadline5"></a>

After composing our abstractions, how do we use similar syntax or words to
express the same kind of operation on different types of objects? For example:

Suppose there are 2 numbers I want to add and then multiply them by 2.

(\* 2 (+ a1 a2))

This is particular enough, but how do I make this general engough such that:

1.  a1 and a2 could be 2 electrical signals that i want to combine and then
    amplify 2 times
2.  a1 and a2 could be 2 vectors that i want to add and then scale them by 2
3.  a1 and a2 could be 2 polynomials that i want to add and then multiply them
    by 2.

Our language should be able to permit us do this. This is done using a technic
called *Conventional interfaces*. This is just another way of controlling
complexity. Agreed upon ways to express computations:

Ways of using Conventional interfaces:

1.  Generic operations
2.  Large-scale structure and modularity
3.  Object-oriented programming
4.  Operations on aggregates

### Making new languages<a id="orgheadline7"></a>

The third technic of controlling complexity is to pick a new language that
highlights major constructs of the problem we are solving.

1.  Metalinguistic Abstraction

    Talks about how to construct new languages.

    1.  Interpretation APPLY-EVAL
    2.  Example-logic programming
    3.  Register Machines

## Some Questions<a id="orgheadline10"></a>

By now, it is evident that the center of computer science is the effective
decription and management of processes, especially as the systems they describe
get larger and larger. Some questions?

### What do we use to describe processes?<a id="orgheadline9"></a>

We use programming languages to describe computational processes. And the
question goes deeper because languages are formalized by a process in the
first place. More on this.

So languages are basically formalisms for reasoning about the use of certain
kinds of logical expressoins.

A lisp interpreter is a machine that carries out processes described in the
lisp programming language.

Therefore, interpreter X is a language that carries out processes described in
language X.

## The essence of Computer Science<a id="orgheadline11"></a>

Formalizing intuitions about &ldquo;how to knowledge&rdquo;. We observe and pick real world
problems we want to solve. We analyze the problem and realize the solution set
to the problem. Interestingly, all the sub components in our solution set are
imaginery. They can be as good or as bad as we can imagine. Every thing is
idealized.
