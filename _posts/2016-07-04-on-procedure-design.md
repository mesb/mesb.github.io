---
layout: post
title: on procedure design
publish: true
---

# On Procedure Design<a id="orgheadline6"></a>

A procedure can be seen as a pattern for the local evolution of a computational
process. A procedure embodies the rules that enforce the evolution of a process,
its consumption of computing space and time. Also, a procedure contains a set of
coherent statements that rely on one another and together achieve the specific
goal intended by the procedure. To design a procedure, we should consider the
sets of values it receives as input and the set of values it should return as
output. A procedure receives input, manipulates the input and returns suitable
output. Hence to design and implement a procedure, we should pay particular
attention to values received and returned as output.

## Steps for designing a procedure, with an example<a id="orgheadline4"></a>

Designing a procedure called *list-length* using scheme

### State the contract of the procedure<a id="orgheadline1"></a>

Identify the input and output, I/O.
list-length takes as input a scheme list, and returns an integer which is
the length of the list.

### Sepcify the usage of the procedure<a id="orgheadline2"></a>

(list-length l) &#x2013;> Int

### Investigate the nature of the input<a id="orgheadline3"></a>

Express the nature of the input in a useful language.

List ::= () | (Value . List)

A list, in scheme, is either empty or it is made of 2 parts:

-   A value, identified as the car of the list, and
-   A list. The rest of the list, called the cdr of the list.

Consider each possible existence of the list, and construct a procedural
handler for it. This is analogous to writing web applications, where the
nature of requests are investigated, requests routes constructed, and
request handlers implemented for each route.

-   Since a list is either empty or contains a value concatenated to a list:

    List ::= () | (Value . List)

    We begin with the case of an empty list.

    The length of an empty list is zero.

    (if (null? lst) 0): If the list is empty return 0 as its length.

-   A non-empty list as 2 parts:

    (Value . List). A non empty list is made of a value and concatenated to a
    list, which is either empty or made of a value concated to a list, which
    is either empty or made of a value concatenated to a list which is &#x2026;

    The length of a value is the unit, that is it is 1. So the length of a
    non-empty list is the length of the first element, which is a value, plus
    the length of the list that value is concatenated to.

    (+ 1 (list-length lst))

    This step, in this case, is tackled using recursion, but other methods
    would do.

-   Put together all the lessons and constructions from 1) and 2) above and
    package them as your procedure.

    ;; list-length: List &#x2013;> Int

    ;; usage: (list-length lst) = the length of the list

    (define list-length

        (lambda (lst)

            (if (null? lst) 0

                (+ 1 (list-length (cdr lst))))))

At this point we have implemented the procedure, taking into account its forms
and handling them appropriately.

## References<a id="orgheadline5"></a>

1.  Structure and Interpretation of Computer Programs
2.  Essentials of Programming Languages
