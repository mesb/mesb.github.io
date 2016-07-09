---
layout: post
title: On Problem Solving
publish: true
---

# On Problem Solving<a id="orgheadline14"></a>

This note is very similar in spirit to my previous notes of procedure design. I excited by how
much i have missed, and how much I have now resolved to gain from learning from
my mistakes and the mistakes those that came before me. Problem solving is
birth right. It comes with the mind, and like a baby practices till it can walk problem solving
skills increase with practice.

Problem solving, seen objectively, appears to be a garbage in, garbage out
process. If you understand the problem and you solve it correctly, you get a
relatively correct solution. If you understand the problem and proceed wrongly,
you miss the solution. And if you understand the problem and solve it
correctly, you get a solution.

## Understanding the Problem<a id="orgheadline1"></a>

The root of all solutoins. The venerable George Polya in his book *How To Solve
It*, has this to say about understanding the problem:

1.  What is the unkown?
2.  What are the data?
3.  What is the condition?
4.  Is it possible to satisfy the condition?
5.  Is the condition sufficient to determine the unkown? Or is it insufficient Or
    redundant? Or contradictory?

Now I realize with great satisfaction that this is the key to the gates of
heaven and at the same time the key to the gates of hell :-)

I will now use these steps to solve a problem.

## Calculating the size of a tree structure<a id="orgheadline11"></a>

I will now use the problem solving framework to write, in scheme, a procedure
that counts the number of leaves of any given tree.

### What is the problem?<a id="orgheadline2"></a>

Given a tree structure or object, identify the number of leaves or nodes in the tree.

### What is the unkown?<a id="orgheadline3"></a>

The unkown in this case is the number of leaves.

### What are the data?<a id="orgheadline7"></a>

The data are the input and output objects.

-   The input is a tree whose number of leaves I intend to find.
-   The output is the correct number of leaves.

These points reduce to the following:

1.  What is the nature of a tree?

    A tree is a list which is empty or whose elements are either lists or atoms. I
    will now formally describe a tree.

    Tree :== () | (Atom. Tree)

2.  What is the output?

    The output is an integer that signifies the count of the number of leaves or
    atoms in the tree.

    Put together, I will obtain a simple description of the language:

3.  countleaves: Tree &#x2013;> Int

### What is the condition?<a id="orgheadline8"></a>

From the above and upon proper investigation, it appears the nature of the data
present the necessary conditions to consider for this problem. The following
questions will produce a suitable set of conditions for solving These problem.

1.  What happens to an empty tree? The number of leaves in an empty tree is 0.
2.  What happens to an atom? The number of leaves in an atom is 1.
3.  What happens to a sublist? A sublist can be treated as an instance of the
    original problem and 1) and 2) above will apply to its solution.

These questions naturally arise from investigation the existential forms or
morphs of tree objects, that is, from understand the question: &ldquo;what are the data?&rdquo;

### Is it possible to satisfy the condition?<a id="orgheadline9"></a>

Yes, using scheme we can write statements that will handle the conditions
specified above. That is, using predicates we can handle a question such as &ldquo;is
the input an empty list?&rdquo;

### Is the condition sufficient to determine the unkown? Or is it insufficient? Or redundant? Or contradictory?<a id="orgheadline10"></a>

The preceding investigation reveals a relatively sufficient solution to the
problem.

## Now the implementation<a id="orgheadline12"></a>

    Tree ::= () | (Atom . Tree)

    ;; count-leaves: Tree ==> Int
    ;; usage: (count-leaves Tree) ==> Int
    (define count-leaves
        (lambda (tree)
            (cond ((null? tree) 0)
                  ((not (pair? (car tree)))
                       (+ 1 (count-leaves (cdr tree))))
                  (else
                       (+ (count-leaves (car tree)) (count-leaves (cdr tree)))))))

    ;; (define tree (list (list 1 2 3) 3  5 (list 3 4 5)))

    ;; (count-leaves tree) ==> 8

    ;;  (count-leaves '()) ==> 0

    ;; (count-leaves '(1 2 3 4)) ==> 4

Voila! The soution seems to work. It might not be the most efficient solution,
but the framework described above served as a good vehicle for understanding
the problem and the solution at every stage of development. And it feels good.

## References<a id="orgheadline13"></a>

1.  How to Solve It by G. Polya
