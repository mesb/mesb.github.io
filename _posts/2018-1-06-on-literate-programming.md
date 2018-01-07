---
layout: post
title: Notes on Literate Programming
publish: true
---

<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#sec-1">1. Notes on Literate Programming</a>
<ul>
<li><a href="#sec-1-1">1.1. A brief look at programming</a></li>
<li><a href="#sec-1-2">1.2. A brief look at computer programming</a></li>
<li><a href="#sec-1-3">1.3. Computer languages and computer programming</a></li>
<li><a href="#sec-1-4">1.4. Contemporary Computer Programming</a></li>
<li><a href="#sec-1-5">1.5. On the birth of literate programming</a></li>
<li><a href="#sec-1-6">1.6. Platforms supporting literate programming</a></li>
<li><a href="#sec-1-7">1.7. An example of literate programming</a>
<ul>
<li><a href="#sec-1-7-1">1.7.1. Problem definition</a></li>
<li><a href="#sec-1-7-2">1.7.2. My exploration of the problem</a></li>
<li><a href="#sec-1-7-3">1.7.3. Algorithm for the maximum element problem</a></li>
<li><a href="#sec-1-7-4">1.7.4. A plain implementation of the algorithm above in Ocaml</a></li>
<li><a href="#sec-1-7-5">1.7.5. Implementation of the maximum finder algorithm in ruby</a></li>
<li><a href="#sec-1-7-6">1.7.6. Some interesting observations</a></li>
<li><a href="#sec-1-7-7">1.7.7. Applying the lessons from above to the other 4 lists</a></li>
<li><a href="#sec-1-7-8">1.7.8. Extra Musings</a></li>
<li><a href="#sec-1-7-9">1.7.9. Resources for literate Programming</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</div>
</div>
<p> </p>
<hr/>
<br />


# Notes on Literate Programming<a id="sec-1" name="sec-1"></a>

## A brief look at programming<a id="sec-1-1" name="sec-1-1"></a>
In the most general sense, people come across programs in most of
their daily endeavors. The idea of "programs" and "programming" is so
common that hanging out with peers for one or two drinks is termed
a program. And we can address others by telling them, "you too like
program." :-)

In schools, there is the mention of degree programs, sporting programs, and
crash programs.

But what exactly does a program mean?

In the contemporary sense underlined above, a program seems to be a
set of activities or events that are sewn together by some end goal
or objective. The drinking program may have **togetherness** as its
end goal. A university program may have the acquisition of
knowledge as the end goal. In most examples of programs, a bunch
of people come together to achieve a common goal. Some programs are
well ordered and every participant has to obey a set of rules so
that the end goal can be achieved with the least amount of
effort. Rules in such programs also help set participants free, for
if everyone follows rules, then there will be less chances of
conflicts that may otherwise  arise with the lack of essential rules.

Consequently, educators develop programs. Gym teachers, dieticians,
parents, and even restaurant chefs program when they arrange events
and activities for those concerned. The dean of a school and the
rest of the faculty assume the role of programmers when they
develop curricula, both ordinary and extracurricular. The parent
who arranges a household such that the kids wake up in the morning,
brush their teeth, eat breakfast, run to school etc,. is a
programmer. You, and me, are programmers and we are programming
when we plan our days and then perform the activities we enumerated
on our todo lists.

As a result, programming involves organizing a set of activities
that collectively lead us to achieve a certain goal.

## A brief look at computer programming<a id="sec-1-2" name="sec-1-2"></a>
Armed with knowledge that programs and programming in the real
world is just a set of activities that enable us to achieve a
certain goal, we may be able to examine the practice of computer
programming. It may become evident that it is the same thing
pattern activities, but on different platforms.

A computer, as is mostly known, is an electronic device that is
capable of manipulating some kinds of objects known as data. As
such, computers are *data handlers*. The way they handle data and
the operations they perform on the data are contingent on the
particular goals of those involved. When dealing with
numbers, they can perform arithmetic operations. When dealing with
Facebook data, they can keep a list of friends, posts, likes,
photos, videos and notes, among many other possibilities. In its
role as a data handler, a computer assumes many positions and performs
many tasks at super speeds.

But how does the computer get to handle data in the way that is
required?

Answering this question is not different from answering the
question, how does a university get to handle its programs in the way
that is required?

A computer needs a programmer in the same way that a university
program needs a programmer, and there is a hint at the role of the dean and
faculty in programming the university courses and other
programs. In the field of computer programming, a programmer is
required to select the activities or events that constitute the
program under development. The programmer arranges these activities
in the most effective manner, so that the computer will spend the
least amount of resources but achieve the best of the desired
goal. Once the most affordable but efficient set of activities is
selected, the programmer communicates the component activities to a
computer so that the computer support and sustain the program.

Programmers organize activities by specifying and prescribing a set
of instructions that must be carried out under a given program. A
computer is a fast performer and it can follow clearly specified
instructions. Every program one engages in is possible because of
the ability to learn about the underlying activities involved. In the case of
a university, the programmers(faculty) will communicate in some
language the essential features of the program. If students perform
any activities, they do so because they are following the
instructions specified by the programmers(faculty). The same thing
happens in the field of computer programming. The programmer needs
to instruct the computer on the intricacies of the necessary
activities.

## Computer languages and computer programming<a id="sec-1-3" name="sec-1-3"></a>
We use natural languages like the English language, French, Ewondo
and Spanish to communicate as the need arises. Similarly, computer
languages are used for communicating with computers. Every computer
has a mother tongue or dialect that it speaks and understands. We
get the computer to perform tasks by talking to it in its
dialect. Interestingly, the dialect of most computers has the form:

1010110100111101010111110001100110011001100110101110101010101111

That humongous collection of 1s and 0s above is the kind of dialect
a computer speaks. The stream of 1s and 0s above is a sentence in
the computer's mother tongue. A single digit, such as 0 or 1, is
called a *bit*. A bit also refers to a binary digit. The
arrangement of bits like shown above is a sentence to a computer,
and such a sentence communicates  instructions to the
computer. Bits are usually grouped into sets, in the same way that
letters of prominent alphabets are grouped into words that form
sentences. The stream of bits above is made of 64 numbers (0 and
1). A computer may split them into groups, such that each group
gets 8 symbols or bits. The line below shows such a grouping:

10101101, 00111101, 01011111, 00011001, 10011001, 10011010, 11101010, 10101111

Each group of 8 bits is normally known as a byte. A byte is the
standard addressable unit of data in the computer. Every thing that
a computer deals with is converted into patterns of bits. These
bits are then manipulated starting from groups of 8(the byte). For
all we care, the binary sentence above may be instructing the
computer to add 2 numbers and report their results.

Every computer comes with its mother tongue, as mentioned above,
and with a set of operations that it can perform. Each of such
operations can be expressed in its mother tongue. In other words,
the mother tongue of the computer is simply the set of all original
tasks that it can perform. Since each task is symbolized by words
or sentences, the set of its original tasks also make up its mother
tongue. The programmer's job involves combining these native words
and sentences to form more compound sentences while at the same
time, these new compound sentences are instructions for the tasks
we want the computer to execute.

But, as can be observed, 1s and 0s are too primitive for most of us
to comprehend. This observation doubles as a difficulty in using
such a language to truly express ourselves. All hope is not
lost. Since computers are programmable devices, it is possible to
introduce programs that perform nothing but translate instructions
from one language to another. As such, we can get one of those
programs to translate from some language we understanding to the
language the computer can understand. In so doing, we can fully
express ourselves in the languages we are comfortable with and we
can have these translation programs translate our thoughts into the
computer's more primitive language of 1s and 0s.

Programs that perform translations of the instructions of one
program, in one language, to equivalent instructions in another
language are known as compilers and interpreters. From the ground
up, on computer systems, the machine language made of 1s and 0s is
the first language, and other languages are translated to this
machine language. Layers of languages have been created in this
vein, with each layer trying to be more expressive than the ones
below. The first layer above machine language is known as *ASSEMBLY
LANGUAGE*.

Assembly language is a way of using short words from natural languages to
symbolize a bunch of bits. For example, if 1011 means an addition
operation on a computer, then ADD = 1011. Computer operations often
take the form of an operator with a topological arrangement of its
operands. In arithmetic, an addition operation involving the
numbers 2 and 3 has the form 2 + 3;

The numbers 2 and 3 are the operands, and + is the operator.

Computers execute instructions that assume the form of operators
and operands. In essence, each instruction commands the computer to
perform an operation on the supplied operands. However, the
position of the operator differs from the position of the operators
of common arithmetic.

There is a beautiful computer architecture called MMIX that was
designed by Don Knuth, for his fundamental books on computer
programming titled, *The Art of Computer Programming*. MMIX has 3
forms of instructions:

1.  OP $X, $Y, $Z
2.  OP $X, $YZ
3.  OP $XYZ

Where OP is an operator, $X, $Y, $Z are locations to acquire the
operands from.

A concrete example can be seen in the case of addition. Suppose
that the mother tongue of an  MMIX machine has 1111 as the addition
operator. Suppose further that 1101 symbolizes location of one of the operands
and 0101 acts similarly for the other operand, and 1001 is the location
where we want to store the results of adding the aforementioned operands.
Then we instruct the computer to perform the operation with the
sentence below:

1111 1001 1101 0101

In English, these symbols mean ADD the contents of the location
with address 1101 to the contents at location 0101, and then store the
results in the location 1001.

The operation flowed from right to left, operand-wise. That is,
first secure room for the operation specified by 1111(ADD) and then
apply ADD to the rightmost operand, then to the next rightmost, and
finally, deposit the results in the location the is the leftmost
operand.

This simple sentence is hard for us humans, but in assembly
language, we can simply say:

ADD $1, $2, $3 which means ADD the contents at location $3 to the
contents at location $2, and store the results in the location $1.

In this form, we humans can understand the instruction ADD $1, $2,
$3 better than its equivalent expression in machine language, 1111 1001
1101 0101. Assembly language is a kind of symbolism for the more
primitive and cumbersome machine language. However, assembly
language is still too primitive for some of us.

Will it not be better if we can speak in magical language that is a
little closer to
English or French or Esperanto?

Will it not be better to have a language where we can express
ourselves clearly, as opposed to the cryptic forms exposed by
assembly language?

For example, we can ask the computer to make decisions with
sentences like:

if today is a "Sunday" then remind me to go to church

Even if the language we get is not as expressive as shown above,
at least if we can be provided with linguistic facilities for
expressing choices, repetitions, assertions &c,. then we may be
more productive in programming and discussing with the computer.

It is for this reason that more languages were added on top
assembly language. Examples of such languages include:

1.  Lisp   - created in 1958
2.  C      - 1969
3.  C++    - 1979
4.  Java   - 1991
5.  Golang - 2009

The languages above and many other modern programming languages
provide us with better means of expressing operative concepts to the
computer. They also have their compilers and interpreters that
convert the sentences we write into sentences of the underlying
machine language.

## Contemporary Computer Programming<a id="sec-1-4" name="sec-1-4"></a>

As observed above, computer programming involves relaying
instructions to the computer. A set of related instructions all
working for a common goal constitute a computer program. A web
browser, for example, is a program. It is written in some language
and your computer sustains the livelihood of your web browser by
executing a series of instructions whose goal is make sure that the
web browser does what it needs to do.

Programs are engineered almost in the same way other real world
systems like bridges, cars, airplanes, and perhaps buildings are
engineered. They are developed as small pieces that are then
combined to form the emergent artifacts we interact with. The main
difference is that computer programs are abstract
components. Computer programs have as their parts a bunch of
idealized components. All the pieces of a computer program are
ideas we had in our heads that have been reduced to a set of
instructions and were communicated to the computer in the guise of
programs. By its very nature, computer programmers are not limited
by physical constraints such as physical law of gravity.

The law of gravity does not affect a computer per se. That is, the
programmer has a singular opportunity to realize as much as she
can. A programmer is only limited by how much she can imagine. For
the very imaginative person can craft ingenious ideas concerning
the tasks involved in a program and consequently get these ideas to
work. This makes programming a very intellectually rewarding
activity. It makes computer programming support aesthetic values
and events that are comparable to the experiences involved in
works of literature like the composition of poetry, prose, and,
perhaps, Platonic dialogues. After all, for what is worth, we may
be instructing the computer using instructions that the computer perceives
as stanzas or some kind of lyrics.

But how are computer programs written?

I'll show an example.

Suppose that we have a lineup of numbers such that they form a list
or sequence where each of the numbers on the lineup has a unique position,
and we want to write a computer program finds the position of
largest of these numbers. In the field of programming, we shall
begin by trying to abstract the problem. That is, we shall, instead,
seek to write a program that finds the largest number in a list of
limited size, or any finite list of numbers. In so doing, we
consider the lists that such a program deals with to have any
countable number of elements. We may say a list of size "N". And
then we work from there.

An easy method for finding the maximum number involves examining each of
the numbers in the order expressed by the lineup, list or sequence,
and also by keeping track of a current maximum element. For each
number that we examine, we compare it to the current maximum, and
update the running maximum to be the current element should it be
that the element we are currently examining is larger the circulating
maximum number. By the end of the list, we shall have a maximum number.

A typical program to perform this task may be written as
demonstrated below:

    '''
     find_max is a function that receives as input a list of numbers, lst,
     and it returns the position of the largest number in the list.

     A list is a sequence of n elements each with a position in line. The first
     element is at position 0, and the last element is as position n-1.
    '''
    def find_max(lst):
        cur_max = 0 # set default maximum to be the first element
        lst_size = len(lst)  # obtain the number of elements in the list

        # now run through each of the elements and
        # compare the element to the current maximum
        for i in range(1, lst_size):
            if lst[cur_max] < lst[i]:
                cur_max = i # the element at position i becomes new maximum element

        # now all number have been examined. Report cur_max as the result
        return cur_max


     # Examples of running the little maximum finder program above

    # example 1 with 10 numbers
    ex1 = [12, 32, 34, 53, 56, 78, 94, 74, 23, 43]
    pos1 = find_max(ex1)
    print "Maximum element is ", ex1[pos1], " which is at position ", pos1

    # example 2 with 5 numbers
    ex2 = [75, 23.4, 100.456, 34, 54]
    pos2 = find_max(ex2)
    print "Maximum element is ", ex2[pos2], " which is at position ", pos2

Maximum element is  94  which is at position  6
Maximum element is  100.456  which is at position  2

The code snippet above is a small program that finds the maximum
element from a finite sequence of numbers.

The program was written by listing the instructions that the computer
needed to perform in order to give us the result we were
seeking. There was some commentary to tell us what is going on,
such as:


Just like in UEFA Champions League games, commentary helps us
understand what it going on. Similarly, computer programs are often
decorated with comments so that we can still understand what we
meant when we visit the code of a piece of software 1-many years after
we wrote it. Without comments, we risk forgetting what we meant to
do and we also make it difficult for others to understand our
code.

Nonetheless, comments like the ones I added above are rather dry
and I myself may spend more time trying to understand the
operations at a later time. The style of commentary above puts the
human reader last. In the code above, I considered the computer
first and wrote code for the computer to understand, and then I
added some bits of comments to aid a human reader.

Can such a technique for programming and providing commentary be
truly helpful as programs become larger and larger?

The short answer is, it depends but most often such a technique
does not help in very large systems.

Then comes the technique of **Literate Programming**

## On the birth of literate programming<a id="sec-1-5" name="sec-1-5"></a>

Literate programming is a technique of programming in which a
programmer considers herself to be composing a work of literature,
although she may actually be writing computer programs. That is,
the programmer strives to communicate the ideas behind the program
first to a human, and only incidentally to a computer. In effect,
the programmer is like a poet or a diviner who describes the solution to a
problem and perhaps how she arrived at that solution. Then she
seasons the works with actual source code that implement the ideas under
consideration. By such a practice, a computer program ends up being
a work of literature like a book, poem, prose, long essay
etc,. that can be studied by other humans and can also be executed
the computer.

Such a technique for programming is very helpful in teaching young
programmers about the craft. For by studying such a piece of work,
a journeyman programmer can understand the states of mind of the
original programmer and perhaps learn faster and more deeply, in
the same way that one can learn from a History book, or from the
notes of an inventor. The chapters in such a book which also
contain genuine programs may be wonderful for learning the various algorithms that
were used in the program at hand and the various tricks the author
conjured in crafting and managing data structures.

Literate programming was invented by the august Don Knuth
in 1983. He communicated his ideas about Literate Program in a
wonderful paper titled, [Literate Programming](http://www.literateprogramming.com/knuthweb.pdf).

Don Knuth said, "Let us change our traditinal attitude to
the construction of programs: Instead of imagining that our main
task is to instruct a *computer* what to do, let us concentrate
rather on explaining to *human beings* what we want a computer to
do."

Don Knuth developed a wonderful computer program called
TeX. TeX is used to style documents as desired by authors,
especially documents that contain technical symbols and
mathematical formulae. Don Knuth also developed a program called
METAFONT which enables its users to design and produce their own
fonts. These are very complex and monstrous computer programs. Don
Knuth confessed that he would not have been able to develop such
large programs without literate programming. He published a book
titled, Tex, the Program, and another book titled, METAFONT, The
Program. These books are the also the authentic programs and one
can learn from them by reading comprehensible paragraphs and
sections that describe the inner workings of the programs.

At the core, literate programming is practice on platforms that
support methods for typing and styling normal  documents and also
methods and tools for typing the source code of computer
programs. Such platforms are said to support a web of
smaller components, some of which are natural text and others which
are program source code. Once the work is done, the programmer can
extract the code alone and compile it into a working program. The
operation of extracting the source code alone from the web of text
and source code is known as "TANGLING". Tangling is done by using a
command called "TANGLE", supposing one were using the original
platforms Knuth developed.

Also, the programmer can export both the source code and the
descriptive text as a PDF, web page, or some other document format
by running a command called "WEAVE".

In the course of developing a literate program, one can explore the
concepts at hand to the deepest of levels and gain more
understanding.

## Platforms supporting literate programming<a id="sec-1-6" name="sec-1-6"></a>

The original platform that Knuth developed for literate programming
is called **WEB**. WEB is simply a collection of a document
typesetting program and a compiler for the language used. WEB used
Knuth's TeX as the document typesetting program and it used the
programming language, Pascal, as its programming tool. The TeX
program itself was written in the **WEB** system. Don Knuth later
developed **CWEB** which was just a combination of TeX for document
typesetting and the C programming language for writing source
code. However, one can create a literate programming system to
contain any of such pairs. That is, literate program is just the
practice that brings together document preparation and program
construction under one umbrella. Any collection of tools that
achieve such a goal is known to support literate programming.

Today, there are more versatile systems that support literate
programming. The Emacs text editor with the assistance of a mode of
text editing called Org-mode support literate programming. In fact,
Emacs + Org-mode go as far as supporting an almost uncountable
number of programming languages. The WEB system supported Pascal
and the CWEB system supported only C. Emacs + Org-mode can be
configured to support any number of languages. Org-mode provides
the means for typing descriptions or our works of literature, while
the configured languages are used for the programs themselves.

Most interestingly, Emacs + Org-mode enable one to run code as they
are developed. CWEB and WEB systems allow us to develop our
documents and programs, then extract and/or publish the works. We
write, then extract the program's code, run them and fix any
errors. These are separate tasks that require practitioners to
switch modes of operation. Emacs + Org-mode allow craftsmen to execute their
programs in the same space that they compose them. The method of
executing source code or programs in the documents that contain
them is also known as reproducible research. Such a technique allows
documents to come to life via the animated moods of the programs
they contain. In so doing, others can read the documents and, additionally,
experiment with the programs that are supplied but  with their custom
data.

## An example of literate programming<a id="sec-1-7" name="sec-1-7"></a>

Conceivably, it's better to demonstrate the technique of literate programming using
the maximum element example that was described and implemented
above. The sections that follow are an attempt to capture the
express the spirits that subsist in the art of literate
programming. The call for exposition and the capture of thoughts
and techniques in both natural language and code is the goal of the
ensuing sections.

### Problem definition<a id="sec-1-7-1" name="sec-1-7-1"></a>

Given an arbitrarily sized list of numbers, develop a computer
program that will find the index(position) of the largest element
in the list.

### My exploration of the problem<a id="sec-1-7-2" name="sec-1-7-2"></a>

The problem asks us to find the maximum number of any finite list
of numbers. The input is a list of any size in the range 0 to N,
where N is a countable number. Computers are fast, but memory is
expensive and we almost always have access to a finite amount of
memory. So it's important that the collections of data  we deal with are
finite or limited to the amount of space we can handle.

1.  What are some of the areas where this program is helpful?

    1.  A program that finds the maximum number/element in a list is
        very important in educational settings where a professor may
        want to select the best student in her class. The position on
        the list could be the student ID of the students. That is, the
        list could be indexed by the student IDs, and at each position
        identified by a student's ID, the student's overall grade is
        deposited.

        In this way, if number 6 is the position with the highest
        value, then the student whose number is 6 is the best student.

        I attended a boarding institution that had an old tradition of
        rewarding the best 10 students by calling them up a stage of
        glory. Similarly, the last 10 students were called up and I
        guess shame or a motivation to work harder  was their reward.

        The maximum element program can be adapted to find the first 10
        or last 10 students. A naive and straightforward approach involves
        running the program 10 times and removing the maximum element
        that is obtained at each run.

    2.  Suppose one is given a list of all the temperature values for
        the city of Garoua, for the year 2016. The task is to find the
        day with the highest temperature. The program that solves the
        problem above can be adapted to find this maximum temperature.

    In general, there are many applications of the maximum element
    program. The solution to such a program can also be used as one of
    the steps of a sorting program, where an investigator  may want to arrange all
    the elements of a collection in ascending or descending order.

### Algorithm for the maximum element problem<a id="sec-1-7-3" name="sec-1-7-3"></a>

An algorithm refers to the technique that is employed to solve a
given problem. An algorithm is like a prescription of the
instructions and the time to apply them in the whole course of
solving a particular problem. There are often multiple techniques
for solving a problem, and those concerned are often interested in the best
technique that will allow them to use less computing resources,
but, furthermore, enable them to solve the problems in the least time possible.

It is therefore evident that with literate programming the
composition of paragraphs that encompass the considerations and
deliberations involved in securing efficient solutions to
problems.

**An Algorithm for finding max element in a list**

INPUT: List of size n, where n is a nonnegative number
       List of elements has form: X<sub>1</sub>, X<sub>2</sub>, X<sub>3</sub>, X<sub>4</sub>, &#x2026;X<sub>n</sub>.
OUTPUT: The index of the largest element in the list

1.  Set cur-max to 0, that is make the first element the
    circulating maximum
2.  Set current-max-element to X<sub>0</sub>.
3.  set counter to 1; Let "i" be counter. i = 1
4.  test if there are more elements in the list: if i > n-1, go to
    step 8
5.  If Xi less than or equal to the  current-max-element, go to step 7
6.  cur-max = i; current<sub>max</sub>-element = X<sub>i</sub>
7.  Increment counter; i = i+1; go to step 4
8.  Return cur-max as the answer. Terminate program

### A plain implementation of the algorithm above in Ocaml<a id="sec-1-7-4" name="sec-1-7-4"></a>

An implementation in the Ocaml programming language

**Quick notes on Ocaml**
Ocaml is a functional programming language. It is built after the
mathematical idea of functions in which a function is like a
device that receives input and maps this input to a unique value
known as its output. Mathematical functions always return the same
value if they act on the same input. As a result, a mathematical
function is different from the computer science idea of a
function.

In computer programming, functions, especially in imperative
languages, can change the contents that are stored in some
location in memory. Therefore, a function may return different
results even when they are given the same input, for the change in
states of memory may induce the change of results.

Functional programming languages are also known as applicative
languages. Functions are building blocks in functional programming
languages so much so that these functions can be passed as input
to other functions. Functions can also be returned as the output
of other functions. These languages work by applying functions to
arguments without changing memory states.

The first functional programming language is LISP and LISP was
invented in 1958. Many languages have branched off from LISP ever
since in the form of dialects. Ocaml has LISP as an ancestor.

Functional programming languages are very rich in novel techniques
for constructing computer programs. They have the tendency to be
the source of many programming language technologies that are
considered indispensable today. For example, the idea of Garbage
Collection came from LISP. The CONDITIONAL statement that has the
form: IF-THEN-ELSE came from LISP. Many other innovations owe
their livelihood to LISP.

Ocaml has wonderful tools for exploring the shape or form of a
data structure. Ocaml has a facility known as pattern matching
that enables programmers to explore the shapes and layout of a
data structure. For example, a list is a simply a first element
that is joined to the rest of its elements. This remaining
elements happen to be a list.

Therefore a list is either empty or it is made of a first element that
is attached to a list(the rest of the list).

The first element of a list is known as the **HEAD** of the list and
the rest of the list is known as its **TAIL**

The empty list is symbolized as **[]**

**::** means attachment or *cons* in LISP parlance. And *cons*
stands for **CONSTRUCT**.

LIST = [] or **HEAD** :: **TAIL**

That is, a LIST is either **EMPTY** ([]) or it's made of a first
element (**HEAD**) that is attached(::) to the rest of the list, the
**TAIL** of the list.

Now exploring a list is as simple as examining its structure by
applying pattern matching and dispatching particular operations if
a match is met.

More about ocaml can be found [here](https://caml.inria.fr/pub/docs/oreilly-book/).

**Ocaml program for maximum element finder**

    let first_of_list lst = let head::_ = lst in head;;
    let rest_of_list lst = let _::tail = lst in tail;;

    let max_finder lst = let rec max_finder_aux lst max index =
        match lst with
        | [] -> index
        | hd::tl -> if hd > max
                    then max_finder_aux tl hd (index)
                    else max_finder_aux tl max (index+1)
        in let first_elt = (first_of_list lst) and tail = (rest_of_list lst) in
        max_finder_aux tail first_elt 0;;

    (*
       Examples of finding the maximum element using the ocaml code above
    *)

    max_finder [23; 43; 56; 12; 98; 32; 56; 78];;

4

**Commentary on the code above**

An Ocaml list has the form HEAD::TAIL. The underscore symbol(\_) is
used to ignore elements. Hence, **head::\_** means ignore tail and
return only the head of the list. Similarly, **\_::tail** means,
ignore the head and return the tail.

The **let** keyword is used to create variables or locations in
memory that store values. Functions are data values too in Ocaml,
hence, **let** is the unified technique for defining both functions
and what is normally called data.

Most functional programming languages, especially the purely
functional ones, do not present explicit linguistic constructs for
looping. They often lack **while**, **do while** and **for**
statements. Instead the rely the recursion and the ability to
perform certain actions upon the state of affairs  of certain
conditions.

The **rec** keyword signifies that the coded and tagged function
will run by calling itself, by itself, as one of the steps in
solving the given problem. Such is the nature and beauty of
recursion.

Pattern matching exists in more than one form in Ocaml. The first
was observed and explained above: **head::\_** and **\_::tail**. The
**match** keyword is an explicit linguistic construct for dissecting
a data structure and to perform suitable actions on its parts. In
the code above, there are 2 prominent patterns:

1.  The Empty List (**[]**) at which point the program terminates or
    the iteration through the components of the data structure come
    to an end. In the code above, the **index** of the maximum number
    is returned.

2.  The pattern for the populated list. A populated list has a
    \*HEAD\*(hd) and a \*TAIL\*(tl). In the code above, *hd* is compared
    to the current maximum element. The same function, max<sub>finder</sub>,
    is recursively called to operate on the *tl* of the
    list. However, if *hd* is bigger than the current max, the new
    call will be applied on the *tl* of the list with *hd* as the
    new maximum element. If *hd* is less than or equal to the
    current maximum element, then the function smoothly operates on
    the *tl* of the list and on the old maximum element. At and
    after each recursive all, the list is reduced by its *hd*,
    therefore, it is reduced by 1, until it the empty list is
    encountered, whence the recursion stops.

The keyword **in** is the Ocaml technique for specifying scopes. In
other languages like C, C++, and Java, code components are often
house in other components and brackets play the role of boundary
markers. A variable in a function is in that function by virtue of
its existence within the curly braces that delimit the said
function. In Ocaml, the **in** keyword means a certain element
should be used and belongs to the scope of another.

And that brings us to the end of the core facilities of the
beautiful Ocaml language.

To continue this reprobate demonstration of literate programming, the
next task is to implement the same algorithm in a different
programming language. Ruby is a modern programming language, very
suitable for web development and for systems administration. It
has ready-made libraries of quality code that are applicable in a
wide range of tasks like text processing, database management,
network management, and rapid prototype testing.

### Implementation of the maximum finder algorithm in ruby<a id="sec-1-7-5" name="sec-1-7-5"></a>

    max_index = 0
    len = lst.length

    if len <= 0
        then return -1
    elsif len <= 1
         then return max_index
    else
        max = lst[max_index].to_i
        rest = lst.slice(1, lst.length)
        i = 1

        rest.each do |elt, index|
        e = elt.to_i
        if e > max then
            max = e
            max_index = i
        end
        i = i + 1
     end
     return  max_index
     end

    -1

A simple code block that prepares a list of numbers.

    l= [34, 54, 12, 89, 23]

| 34 | 54 | 12 | 89 | 23 |

    3

### Some interesting observations<a id="sec-1-7-6" name="sec-1-7-6"></a>

Literate programming on Emacs + Org-mode allows a practitioner to use
different languages for different tasks and equally allows
stakeholders to share data from programs that are implemented in
different languages. In Emacs + org-mode a craftsman can use the output of
one program in a given language as the input of another program that
written in a different language.

**Example**:
It is tedious to manually create the lists that I want to use for
the maximum element problem.

I'd love to write a function that generates a list of elements
that are chosen at random.

All I'll need to do is supply the number of elements I want in the
list.

The program receives an empty list, for a start, and the number of
elements, n, to generate and fill the list with. It then returns a
list of n randomly generated numbers.

Now I won't have to worry about manually creating a list.

And I can use the list generated by this little program on any
other programs that receive lists, no matter the language they are
written in.

    let rec make_list_elts lst n =
        if n = 0
            then lst
        else
            let temp = Random.int 534 in
            make_list_elts (temp::lst) (n-1);;

    make_list_elts [] 10;;

    - : int list = [302; 410; 118; 416; 337; 386; 298; 410; 48; 459]

Now there is this little idealized  device called **make-list** that
generates random numbers. So one can test the max finder
program on the lists that **make-list** generates.

A good test, as demonstrated below, involves creating 5 lists and
using them as this note unfolds.

**Examples of using make-list**

    let list1 = make_list_elts [] 10;;
    let list2 = make_list_elts [] 15;;
    let list3 = make_list_elts [] 20;;
    let list4 = make_list_elts [] 25;;
    let list5 = make_list_elts [] 30;;

It may also be helpful to write a function that prints the
elements of a list, so that one can know the elements of any given
list

    let rec list_printer lst =
        match lst with
        | [] -> print_newline();
        | hd::tl -> (print_endline (string_of_int hd)); list_printer tl;;

    <fun>

Another little device that displays the contents of a given list.

At this point, the elements of a list can be printed and the
various lists that are printed can be captured on this current file.
The results are captured in the form of universal list, at least in
the universe of Emacs + Org-mode.

Once the elements are presented  as universal lists, any other
program in this file can use the results.

**A display of the elements of list1**

    list_printer list1;;

    - 465
    - 109
    - 52
    - 128
    - 473
    - 478
    - 323
    - 302
    - 165
    - 515
    - - : unit = ()

**A display of the elements of list 2**

    list_printer list2;;

    - 46
    - 79
    - 269
    - 438
    - 433
    - 397
    - 276
    - 404
    - 30
    - 487
    - 184
    - 110
    - 175
    - 181
    - 134
    - - : unit = ()

**The elements of list3 are presented below sing the list-printer program**

    list_printer list3;;

    - 322
    - 49
    - 157
    - 217
    - 95
    - 41
    - 327
    - 477
    - 227
    - 266
    - 67
    - 58
    - 508
    - 158
    - 430
    - 363
    - 183
    - 198
    - 131
    - 100
    - - : unit = ()

**A display of the fourth list that was randomly generated**

    list_printer list4;;

    - 279
    - 66
    - 133
    - 162
    - 213
    - 522
    - 83
    - 204
    - 18
    - 21
    - 399
    - 255
    - 427
    - 0
    - 44
    - 372
    - 402
    - 279
    - 82
    - 197
    - 405
    - 155
    - 461
    - 9
    - 415
    - - : unit = ()

**And finally the last list, list 5 is displayed yonder**

    list_printer list5

    - 157
    - 174
    - 74
    - 183
    - 368
    - 142
    - 278
    - 255
    - 226
    - 145
    - 328
    - 236
    - 511
    - 203
    - 20
    - 238
    - 473
    - 277
    - 77
    - 495
    - 201
    - 285
    - 6
    - 319
    - 488
    - 458
    - 163
    - 96
    - 133
    - 256
    - - : unit = ()

At this point, the various lists: list1, list2, list3, list4,
list5 have all been converted to Org-mode lists. However, there is
a small problem. Ocaml is a functional programming language by
birth, but it was patched up with features of imperative languages
like C. That is, it was extended to accommodate non-functional
techniques. Therefore, one can nevertheless program by changing memory using
Ocaml when the need arises. These features where added so that
programmers can also represent algorithms that are fundamentally
imperative in nature. For example, reading and writing to files is a task
that involves changing memory contents. A purely functional
approach for file operations and other Input/Output operations
will be too expensive.

As a result, the construct, **unit=()** was introduced to Ocaml. When
a string is printed, the last object printed is **unit=()**. In the
examples above, **unit=()** will be attached to the end of the printed
lists. So accommodations have to be made to get rid of them. A
possible solution may be to rewrite the printing function in
another language that is cut  out for the job. And that's the
advantage of using a literate programming environment such as
Emacs + Org-mode. One can use the best language for the cabinet of
tasks that come by.

However, this note has as its main purpose the demonstration of
literate programming. Instead, we'll use another language to get
rid of **unit()** at the end of all our lists.

Python is suited for this task. We can use python's list
slicing mechanisms to get rid of the last elements of the lists as
shown below.

But, ruby has deplorable tools for examining the elements of an
object. So let's first of all examine the contents of one of the
lists using ruby, so that we can decide how to delete **unit=()**

Better still, we can observe the type of the lists and
consequently manipulate appropriately.

There is the need for  a small ruby program that returns the type/kind
 of information list1 stores.

    puts lst.class

    String

The *class* of an object tells of its kind/type.

The result reports that lst=list1 is of type String.

This implies that Emacs + Org-mode received the list from Ocaml in
this text document and automatically converted that result into
text format. That's unexpected, but it leaves room for more fun
investigations and exploration of literate programming.

The next task in line is to inspect the elements of the list in
order to understand how Org-mode configured them. Ruby has a good
tool called *inspect* that returns the internal representation of
a data object.

    puts lst.inspect

    "465\n109\n52\n128\n473\n478\n323\n302\n165\n515\n\n- : unit = ()"

The result shows that the elements are combined into 1 single
string, but each individual element is demarcated from the next
with the "\n"(the newline character). Hence, the elements are
arranged in a sequence that has a vertical orientation.

All the elements of the list above are strings, that is,
collections of characters. We therefore have to go through all of
them if we have to eliminate ": unit = ()"

One simple way to solve this problem is to split the string
above. We can collect every element before "\n" into a new list as
shown below. Ruby has a function called split(separator) that
splits a string into its component elements, where the separator
is like the joint where the split function applies its slicing.

    result = lst.split("\n")
    puts result.inspect
    puts result.class
    puts result[0]

    ["465", "109", "52", "128", "473", "478", "323", "302", "165", "515", "", "- : unit = ()"]
    Array
    465

Splitting the string of characters at the "\n" joint disorientates
the vertical arrangement. The "\n" makes the next element assume
the first position on a new line. Hence, getting rid of it
enforces a more horizontal orientation of the elements.

The inspection above tells us that ""(the empty string) occurs after the last
number. Hence, we can eliminate the sub list that starts with ""
up to the end of the original list. The inspection also tells us
that the result of splitting list1 at the "\n" joints returns a
result that is an array or a list or strings.

Perhaps, we can now split the string at every "\n" and determine
where to start eliminating data.

We can do that by saving the results of splitting list1 in a data
object called *result*. Then the next step is to determine how far away "" is
from the last element, and then chopping off data from that position.

    result = lst.split("\n")

    i = 0;
    result.each {
        |elt|
        puts "#{elt} is at position: #{i}"
        i += 1
    }

    465 is at position: 0
    109 is at position: 1
    52 is at position: 2
    128 is at position: 3
    473 is at position: 4
    478 is at position: 5
    323 is at position: 6
    302 is at position: 7
    165 is at position: 8
    515 is at position: 9
     is at position: 10
    - : unit = () is at position: 11

The result above shows that the last element is "- : unit = (),"
and the last but one is "". So we can eliminate the last 2
elements.

Before performing surgery on the the list obtained above, it may
be wise to print the list normally, without the indices, to get
another view of how the elements are currently arranged in memory.

We can do that using python

    results = lst.split("\n")
    print results

['465', '109', '52', '128', '473', '478', '323', '302', '165', '515', '', '- : unit = ()']

As expected, the resulting object is an array. Note that the code above is
python, while the first time we split the string we used ruby.

We now have a list of the elements, but in the same form that
Ocaml originally produced. It looks like we are wasting time going in
circles with these lists, but, again, the main purpose is to demonstrate the
power of literate programming and how it can be used to experiment
on programs and data structures.

We could have originally used ocaml to get rid of "-: unit = ()",
but I think it's more fun to explore and continue the task with
different languages.

We can now eliminate the last 2 elements of the list using
python's facilities for slicing strings.

    results = lst.split("\n")
    list_length = len(results)
    result = results[0:list_length-2]
    result = [int(x) for x in result]
    return result

<table width="100%"  border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />
</colgroup>
<tbody>
<tr>
<td class="right">465</td>
<td class="right">109</td>
<td class="right">52</td>
<td class="right">128</td>
<td class="right">473</td>
<td class="right">478</td>
<td class="right">323</td>
<td class="right">302</td>
<td class="right">165</td>
<td class="right">515</td>
</tr>
</tbody>
</table>

After slicing off the unwanted data, a clean an fresh list is
returned.

A quick test of the *max-finder-ruby* function on the newly
prepared list. And it works.

    9

And voila! We have a clean list without any "" or  "- : unit = ()"

### Applying the lessons from above to the other 4 lists<a id="sec-1-7-7" name="sec-1-7-7"></a>

We have seen how to eliminate irrelevant data that was introduced
by Ocaml. We can now apply the same operations to the other
lists.

In fact, we can begin from scratch and apply the operations to the
the  4 lists, using different languages, thereby creating new
blocks of data with clean lists and operating on them.

There is the possibility for the use of C, C++, PHP, Bash, Java for this
task, provided Emacs + Org-mode is configured to handle the
languages.

**The first run is on list2 and the python language is again employed.**

    results = lst.split("\n")
    list_length = len(results)
    result = results[0:list_length-2]
    result = [int(x) for x in result]
    return result

<table width="100%" border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />
</colgroup>
<tbody>
<tr>
<td class="right">46</td>
<td class="right">79</td>
<td class="right">269</td>
<td class="right">438</td>
<td class="right">433</td>
<td class="right">397</td>
<td class="right">276</td>
<td class="right">404</td>
<td class="right">30</td>
<td class="right">487</td>
<td class="right">184</td>
<td class="right">110</td>
<td class="right">175</td>
<td class="right">181</td>
<td class="right">134</td>
</tr>
</tbody>
</table>

**The maximum element of the sequence is captured below**

    9

**The second run is on list3. The list is clean and the max  element extracted**

    results = lst.split("\n")
    list_length = results.length
    result = results.slice(0, list_length-2)
    return result

<table width="100%" border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />
</colgroup>
<tbody>
<tr>
<td class="right">322</td>
<td class="right">49</td>
<td class="right">157</td>
<td class="right">217</td>
<td class="right">95</td>
<td class="right">41</td>
<td class="right">327</td>
<td class="right">477</td>
<td class="right">227</td>
<td class="right">266</td>
<td class="right">67</td>
<td class="right">58</td>
<td class="right">508</td>
<td class="right">158</td>
<td class="right">430</td>
<td class="right">363</td>
<td class="right">183</td>
<td class="right">198</td>
<td class="right">131</td>
<td class="right">100</td>
</tr>
</tbody>
</table>

    12

**The fourth run on list4 uses Ocaml again, although with some tricks**
Ocaml is a very beautiful language. I'm going to use some of its
powerful features below and then make brief description of those
features.

    #load "str.cma";;

    let reg_pat = (Str.regexp "\n") in
    let new_lst = (Str.split reg_pat lst) in
    let len = ((List.length new_lst) - 2) in

    let (res, _, _) =
         List.fold_left
             (fun (acc, ctr, max)  hd
                       ->
                        if ctr < max-1
                            then (acc@[(int_of_string hd)], (ctr+1), max)
                         else
                            (acc, ctr, max))
                   ([], 0, len) new_lst
                              in
                             (max_finder res);;

<table width="100%" border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />
</colgroup>
<tbody>
<tr>
<td class="right">279</td>
<td class="right">66</td>
<td class="right">133</td>
<td class="right">162</td>
<td class="right">213</td>
<td class="right">522</td>
<td class="right">83</td>
<td class="right">204</td>
<td class="right">18</td>
<td class="right">21</td>
<td class="right">399</td>
<td class="right">255</td>
<td class="right">427</td>
<td class="right">0</td>
<td class="right">44</td>
<td class="right">372</td>
<td class="right">402</td>
<td class="right">279</td>
<td class="right">82</td>
<td class="right">197</td>
<td class="right">405</td>
<td class="right">155</td>
<td class="right">461</td>
<td class="right">9</td>
<td class="right">415</td>
</tr>
</tbody>
</table>

22

**Some powerful features of Ocaml**
The most prominent feature in the code above is the
*List.fold<sub>left</sub>* function. It's simply a mechanism for walking
through the elements of list, processing each element and adding
the results to another structure called an
accumulator. Interestingly, Ocaml provides a powerful typing
system, so one can create custom types and extend them as needed.

As such, the accumulator above is a collection of three separate
objects (acc, ctr, max). There is the accumulator itself, which is just a
growing list of all the elements, except the data pieces we sought to
delete. Then there is a counter and a max counter. The program stops
going through the list elements when the counter becomes 1 unit
less than the max.

(res, \_, \_) is means of matching the objects that List.fold<sub>left</sub>
returns. That is, (acc, ctr, max); however, (res, \_, \_) means
ignore ctr and max, and return just the *res* object, which
stands for the accumulator. The other pieces were temporary workers.

**The last example is done in emacs-lisp**

    (require 'cl)
    (setq res (split-string lst))
    (setq len (length res))
    (subseq res 1 (- len 5))

    8

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />

<col  class="right" />
</colgroup>
<tbody>
<tr>
<td class="right">109</td>
<td class="right">52</td>
<td class="right">128</td>
<td class="right">473</td>
<td class="right">478</td>
<td class="right">323</td>
<td class="right">302</td>
<td class="right">165</td>
<td class="right">515</td>
</tr>
</tbody>
</table>

    8

**Emacs-Lisp**
Emacs-lisp is a dialect of LISP that serves as the main scripting
language for the Emacs text editor. In effect, Emacs-lisp is
comparable to Javascript in the web browser. However, Emacs-lisp has a
more fundamental role to play on the wonderful text editor.

Emacs is known to be the Tinkerer's editor. It's an editor that
can be configured as much as one can imagine. Its versatility and
adaptability is owed to Emacs-lisp. Emacs itself is a giant LISP
interpreter, with the assistance of Emacs-lisp. Source code can be scribbled
anywhere on the text editor and immediately executed. All the
essential Emacs APIs have endpoints that are accessible as
Emacs-lisp functions.

### Extra Musings<a id="sec-1-7-8" name="sec-1-7-8"></a>

The problem of finding the maximum element in a list is interesting
but very simple. One may wonder why it took so many pages for such
a simple task. The matter at hand was the exploration of the
methodology of literate programming, which provides a swift
vehicle for navigating the wonders that lay underneath algorithms
and data structures. When one is engaged in a session of literate
programming, the zeal to understand a problem becomes natural, the
ability to pen one's thoughts are right beneath the fingers and
the paragraphs, lists, side notes and all what not that are penned
in the process testify to the utility that this methodology adds
to a programmer's experience.

A typical biologist may spend great amounts of time in her lab,
studying organisms of interest and capturing their every
maneuver. A cosmologist will spend immense amounts of time
exploring the starry skies and collecting suitable data. She will
then analyze them in an attempt to understand some underlying
patterns. And the delighted and delightful mathematician may need a pack of pens
and a large sheet of paper to capture the patterns that underlie
mathematical objects like the Icosahedron. Countless other
occupations envelope joyous activities. It seems it's part of our
birth right as humans to search for perfection and the
beautiful. The rational parts of ourselves continually lead us to
investigate and ponder on the ever so subtle infinite processes
around us.

And now, the computer programmer, armed with computer languages
and blessed with a multifaceted and resourceful text editing
platform, can enjoy the same wonders a cosmologist or mathematician
would enjoy. With a multi-programming platform like Emacs +
org-mode, one can investigate very deeply the inner workings of
computer algorithms and tinker with them and with data structures
alike, in the same way a physicist scrutinizes theorems until she
arrives at indispensable, indescribable but ever relevant first
principles. The arts of experimentation and investigation are both
enjoyable and painful, but the better the tools at hand, the more
enjoyable every step becomes.

Most of the code written above is irrelevant. The little functions
that we composed were not the most efficient, the process of
conceiving them and bringing them to life surpasses their final
form they've taken. Moreover, as an exercise of the venerable art
of literate program, the programs written above are akin to some
draft documents that perhaps an essayist or some poet may decide to
give a shot at, as a recreational activity. But on the most
serious note, literate programming provides a platform on which
one can think deeply and capture the thoughts at the same time,
while also verifying, with the assistance of runnable source code,
the sudden bursts  of insights that arrest those engaged in deep
thinking.

A huge part of computer programming involves the analyses of the
algorithms that are related to a given problem. Yes, it is good to
scribble down ideas and it is wonderful to brainstorm.

But what is the difference between brainstorming and veritable
development of *the* project?

One of the most essential features of literate programming is the
development of comprehensive and comprehensible documentation for other humans,
including the programmer herself, especially many moons after the
program was developed. Software is always very complex to
build. They get complex briskly and they grow large, fast enough,
so much so that it becomes impossible for one person to have all
the aspects of some software in her head at once. Proper documentation is one
method that alleviates most of the confusion and pains of the
spartan craft of software development. But imagine capturing the
exact understanding behind a given procedure in some descriptive
form, as if you were writing a book for your future self and for
others. Such and many more are the benefits of literate programming.

### Resources for literate Programming<a id="sec-1-7-9" name="sec-1-7-9"></a>

1.  [literate programming web resources](http://www.literateprogramming.com/)

2.  [Knuth 1983](http://www.literateprogramming.com/knuthweb.pdf)

3.  [Wikipedia Page](https://en.wikipedia.org/wiki/Literate_programming)

4.  [The Emacs Editor](https://www.gnu.org/software/emacs/)

5.  [Wikipedia Emacs](https://en.wikipedia.org/wiki/Emacs)

6.  [Org-mode page](https://orgmode.org/)

7.  [Org-mode Wikipedia Page](https://en.wikipedia.org/wiki/Org-mode)
