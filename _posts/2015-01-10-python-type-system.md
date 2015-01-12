---
published: false
---

## Overview<a id="sec-1-1"></a>

Types are at the center of computing. Types represent the things or objects we
deal with in computing. A data type is a set of objects, and the permissible
operations performable on these objects.

Naturally, languages are used to convery information. The senders and receivers
of these information have processing capabilities that help them to lexically
understand information. Unlike natural communication, computing relies on
pre-preprocessed lexicons. A computer language is built and taught to a
computer, so that it can then have a compiler or interpreter make sense out of
its use.

Typically, every piece of information or data object passed around a computing
process must be explicitly described to the computer. The processor must keep
an account of these objects so that computations can be done right. This
rightness of computation is ensured by:

1.  Letting the programmer define the types of objects:
    This is typical of statically typed programming languages. In such
    languages, examples being C, C++, Java and Golang, variables are the
    entities that are tagged with types. Programmers define variables with
    specific types, and these variables store suitable data objects.

2.  The run time takes care of types of objects:
    This is where most dynamic programming languages fall. Python, Lisp,
    Javascript, ruby, Perl etc. Everything in such languages are objects, and
    most of them are immutable. Each object is unique, and the types are
    dynamically managed by the intepreter at run time. Variables are just
    references to these objects.

With all of these, we can dive into Python's dynamic type system.

## Use variables and objects<a id="sec-1-2"></a>

Each piece of data in a python program is an object. '3' for example is an
object.

When we say age = 25, we are assigning a reference called 'age' to the
object 25. So the type is tied to the object. This makes variable assignment,
and manipulation the work of the interpreter, as opposed to the manual
assignment/management of such task by the programmer.

So, 25 is an object managed by Python. It has a type, a reference count, and other
metadata used by python.

Most importantly, there exist metadata used by the garbage collector.

## References, copying<a id="sec-1-3"></a>

Since everything is an object, assignment means assigning references to
objects. So if we assign a variable to another variable, we are evaluating an
expression, and the resulting value(object) stored in the first variable ends
up being referenced by the second variable.

Primitive data objects are immutable, meaning the value or object 3 can never
be changed. It will always be 3. Hence,

a = 3

b = a

a = 5

does not changed the object pointed to by b. All what happens is, a now points
to 5, while b points to the value(object) 3.

However, mutable compund data types like lists, dictionaries, sets and maybe
files observe this kind of manipulation differently. They permit in place
mutation. Meaning, one of the values in a sequence can be changed, and all
varibales pointing to that sequence will be updated.

e.g

items = [1,2,3,4,5]

itemsBackup = items

`items[2]` = 4

means itemsBackup will automatically reflect the changes made. This can cause
serious bugs in programs. This should be avoided by using copy operations.

itemsBackup = items[:]

This operations results in the copying of the members of items into
itemsBackup and changing any won't affect the other.

Note that, this slicing method won't work in all cases. So we might want to use
the built in "copy" module to effect such operations.

import copy

Y = copy.copy(X)

and to copy nested data use:

Y = copy.deepcopy(X)

## Garbage collection<a id="sec-1-4"></a>

Each object has a type, and a reference count. Creating an object means
 incrementing its count. The runtime watches the count of
objects, and when the count drops to zero, it implies that the object is no
more needed, and the garbage collector eventually frees up the object from
memory.

For example,

year = 2014

The code above creates a variable called year that references the
object 2014. Python creates a count of let's say 1 for the object 2015.

Now let's reassign the variable:
year = 2015

year now references the object 2015. The reference count for the object 2015 goes to 1,
while the count of 2014 drops to 0. Therefore, the garbage collector will free
up the location in memory where 2014 was stored.

As the case may be, it can be costly to free up memory like that in some types
of programs. Python therefore caches small objects like integers so that
programs can run faster, and reduce overhead cost.

That in a nutshell is how the python garbage collector works.