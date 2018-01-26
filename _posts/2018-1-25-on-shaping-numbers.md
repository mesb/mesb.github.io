---
layout: post
title: Playing with numbers and shaping them
publish: true
---

# Table of Contents

1.  [A brief rant on the numbers](#orge0f3652)
2.  [Displaying the sum of a sequence of numbers](#orgd6636d8)
3.  [Summing the first n odd numbers](#org5334f8b)
4.  [Redisplaying the sum of the first n numbers](#orgf3ca0d9)
    1.  [Code section for the desired display](#orgd1365c1)
5.  [Conclusion](#org1009e63)



<a id="orge0f3652"></a>

# A brief rant on the numbers

**Who can live without numbers?**

**Better still, what is a number?**

The idea of numbers has fascinated humans for centuries and will
continue to do so for ages to come. Numbers, at least in symbolic
form, are akin to clothing that we put on magnitudes or quantities.
Quantity is contemporarily taken to denote things that can be increased
or decreased. The temperature of today can be represented using
quanities. But the other fluid idea that enables our comprehension
of the increase or decrease of quantities in question are nothing
but an embodiment of our conception and manipulation of numbers. At
deeper levels, perhaps, the metaphysical, and depending on whom you
ask, numbers are a fabric upon which our
whole cosmos is erected. An ancient Greek sect, known as the
Pythagoreans, worshipped numbers.

The applications of numbers are evident in a wide range of domains.
Distance, displacement, brokeness, richness, temperature, age, and
an **immeasurable** complex of other notions are expressed using
numbers. Added to their ubiquity is the immense wealth of knowledge
that humans have accumulated and will continue to accumulate in
designated and related fields, the sciences in particular, that use
numbers as currency. If arithmetic were perceived as a boardgame, say like
chess or checkers, then numbers will be the pieces, and the
operations called addition, subtraction, multipication and division
will be akin to the various moves that the game pieces, numbers in
this case, can engage in. We, as players of the game, will move
these pieces and convert them into other types of pieces with the
assistance of the said operations.

In chess, for example, there are certain moves that oversee the
promotion of a pawn to higher ranks like queen, knight, rook or
bishop. Perhaps, adding 1 to 2 oversees a promotion of one of them
to 3. In effect, the arithmetic operations permit us, the players,
to reconfigure numbers, create new ones from old ones, dismantle
others as in the case of division, combine some as is the case of
multiplication and perhaps make some disappear as in the case of
subtraction. Kids and those who've been kids before may have
experienced some good moments while learning to count using sticks,
pebbles, and other toys that are suitable for such. In using
these objects to learn how to count and operate on numbers, there
was the chance to rearrange these pebbles into rows and/or columns.

It's time for a silly game. Suppose that we can represent numbers
using discrete objects that we shall symbolize by dots, asterisks
and perhaps some interesting characters. One dot or asterisk would
symbolize the number 1. Two dots will symbolize the number 3, and
so on. With that in place, what happens if we try to arrange these
dots(numbers) in different orientations as we perform some playful
operations of addition on them.

The table below shows the first 10 numbers as arrangements of a
sequence/line of big dots.

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-right">Number</th>
<th scope="col" class="org-left">Dot Representation</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-right">1</td>
<td class="org-left">o</td>
</tr>


<tr>
<td class="org-right">2</td>
<td class="org-left">o o</td>
</tr>


<tr>
<td class="org-right">3</td>
<td class="org-left">o o o</td>
</tr>


<tr>
<td class="org-right">4</td>
<td class="org-left">o o o o</td>
</tr>


<tr>
<td class="org-right">5</td>
<td class="org-left">o o o o o</td>
</tr>


<tr>
<td class="org-right">6</td>
<td class="org-left">o o o o o o</td>
</tr>


<tr>
<td class="org-right">7</td>
<td class="org-left">o o o o o o o</td>
</tr>


<tr>
<td class="org-right">8</td>
<td class="org-left">o o o o o o o o</td>
</tr>


<tr>
<td class="org-right">9</td>
<td class="org-left">o o o o o o o o o</td>
</tr>


<tr>
<td class="org-right">10</td>
<td class="org-left">o o o o o o o o o o</td>
</tr>
</tbody>
</table>

The shape traced by the table above reveals the form of a triangle.
This form may be more evident if we erase the table's headers and
first column.

    *
    * *
    * * *
    * * * *
    * * * * *
    * * * * * *
    * * * * * * *
    * * * * * * * *
    * * * * * * * * *
    * * * * * * * * * *

The form assumed by the arrangement of asterisks above traces a
triangle. In effect, the numbers from one to ten have been lined up
such that each number, say the number 2, is on the second line and
the number 3 on the third line, and so on. This reveals some
interesting properties of numbers that can be explored further,
alongside some additionally awe-inspiring operations.


<a id="orgd6636d8"></a>

# Displaying the sum of a sequence of numbers

The table and triangle that was observed above can be considered to
represent the sum of numbers from a given number that's designated
as the start number, to the another given number that marks the
end. For example, suppose we want to add all numbers from 1 to 5.
It's easy to use the asterisk symbol and the technique shown above. One
can write 1 asterisk for the number 1, and then add 2 to 1, by
writing 2 asterisks on the next line etc,.

In the light of the adding consecutive numbers as lines represented
by a collection of asterisks the size of the magnitude of the number
in question, we can shape these sums and reveal interesting
geometric objects. In the same manner, we may say that  we are shaping
numbers.

As an exercises of this concept, consider summing 1 to 5. The
arithmetic representation of this operation is:
\( 1 + 2 + 3 + 4 + 5 = 15 \)

The asterisk representation will be:

\( * + * * + * * * + * * * * + * * * * *
  = * * * * * * * * * * * * * * * \)

Suppose further that the plus(+) symbol is used in this game to
signify the beginning of a newline and the numbers(asterisks) after
any plus symbol should be placed on the next line. Doing such will
leave us with:

    *
    * *
    * * *
    * * * *
    * * * * *

And the sum total of these asterisks is 15.

This is an example of a more general operation called finding the
sum of the first **n** numbers. So far, we've obtained the sum of the
first 10 numbers, in first table above, and now the sum of the first
5 numbers, as shown in the results above. The sum in this case is
the total number of asterisks that we can count from the game of
representing and summing numbers using asterisks and newlines for
plus symbols.


<a id="org5334f8b"></a>

# Summing the first n odd numbers

The stupid games above involved summing the positive whole numbers
in increasing order.

What if one were to examine the numbers in increasing order, but
eliminate all the even numbers. Perhaps, we'd obtain a numberline as
shown below:

1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21, 23, 25, 27, 29, 31, &#x2026;

That is, we've eliminated:

2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, &#x2026;

It's also evident that the odd numbers above are generated by
continuously adding 2 to a given predecessor of a number, where the
first number, and original predecessor, is 1. As such, 1 + 2 = 3,
and adding 2 to 3 yields 5, which then consumes another 2 to form 7,
and so on.

Now, what happens if we sum this lineup of numbers?

1 + 3 = 4
4 + 5 = 9
9 + 7 = 16

The first 3 sums above show something interesting. The sums are the
squares of the numbers 2, 3, and 4.

If we add the next odd number, that is 9, to the last sum above,
which is 16, we obtain 25 and 25 is the square of 5.

Hence we can obtain the squares of the first **n** numbers simply by
playing with the first **n** odd numbers. Now, let's use the asterisks
notation to draw of display these numbers.

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-right">Number</th>
<th scope="col" class="org-left">Sum</th>
<th scope="col" class="org-left">Presentation</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-right">1</td>
<td class="org-left">0 + 1</td>
<td class="org-left">o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">4</td>
<td class="org-left">1 + 3</td>
<td class="org-left">o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">9</td>
<td class="org-left">4 + 5</td>
<td class="org-left">o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">16</td>
<td class="org-left">9 + 7</td>
<td class="org-left">o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">25</td>
<td class="org-left">16 + 9</td>
<td class="org-left">o   o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">&#xa0;</td>
</tr>


<tr>
<td class="org-right">36</td>
<td class="org-left">25 + 11</td>
<td class="org-left">o   o   o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o   o   o</td>
</tr>


<tr>
<td class="org-right">&#xa0;</td>
<td class="org-left">&#xa0;</td>
<td class="org-left">o   o   o   o   o   o</td>
</tr>
</tbody>
</table>

Again, if the table is erased, and if we view them individually, the
form becomes more evident.

    Representation for number  1
    *


    Representation for number  4
    * *
    * *


    Representation for number  9
    * * *
    * * *
    * * *


    Representation for number  16
    * * * *
    * * * *
    * * * *
    * * * *


    Representation for number  25
    * * * * *
    * * * * *
    * * * * *
    * * * * *
    * * * * *


    Representation for number  36
    * * * * * *
    * * * * * *
    * * * * * *
    * * * * * *
    * * * * * *
    * * * * * *


<a id="orgf3ca0d9"></a>

# Redisplaying the sum of the first n numbers

In section 2 above, the sum of the first n numbers was displayed as
a right angled triangle. This section is just a redisplay of those
triangles but in form of isoleces triangles. That is, we shall make
them look like triangles which have 2 sides that are equal.


<a id="orgd1365c1"></a>

## Code section for the desired display

    Representation for the sum of the first 1, number(s)[ 0 ]




    Representation for the sum of the first 2, number(s)[ 1 ]

       *



    Representation for the sum of the first 3, number(s)[ 3 ]

        *
       * *



    Representation for the sum of the first 4, number(s)[ 6 ]

         *
        * *
       * * *



    Representation for the sum of the first 5, number(s)[ 10 ]

          *
         * *
        * * *
       * * * *



    Representation for the sum of the first 6, number(s)[ 15 ]

           *
          * *
         * * *
        * * * *
       * * * * *



    Representation for the sum of the first 7, number(s)[ 21 ]

            *
           * *
          * * *
         * * * *
        * * * * *
       * * * * * *



    Representation for the sum of the first 8, number(s)[ 28 ]

             *
            * *
           * * *
          * * * *
         * * * * *
        * * * * * *
       * * * * * * *



    Representation for the sum of the first 9, number(s)[ 36 ]

              *
             * *
            * * *
           * * * *
          * * * * *
         * * * * * *
        * * * * * * *
       * * * * * * * *



    Representation for the sum of the first 10, number(s)[ 45 ]

               *
              * *
             * * *
            * * * *
           * * * * *
          * * * * * *
         * * * * * * *
        * * * * * * * *
       * * * * * * * * *



    Representation for the sum of the first 11, number(s)[ 55 ]

                *
               * *
              * * *
             * * * *
            * * * * *
           * * * * * *
          * * * * * * *
         * * * * * * * *
        * * * * * * * * *
       * * * * * * * * * *



    Representation for the sum of the first 12, number(s)[ 66 ]

                 *
                * *
               * * *
              * * * *
             * * * * *
            * * * * * *
           * * * * * * *
          * * * * * * * *
         * * * * * * * * *
        * * * * * * * * * *
       * * * * * * * * * * *



    Representation for the sum of the first 13, number(s)[ 78 ]

                  *
                 * *
                * * *
               * * * *
              * * * * *
             * * * * * *
            * * * * * * *
           * * * * * * * *
          * * * * * * * * *
         * * * * * * * * * *
        * * * * * * * * * * *
       * * * * * * * * * * * *



    Representation for the sum of the first 14, number(s)[ 91 ]

                   *
                  * *
                 * * *
                * * * *
               * * * * *
              * * * * * *
             * * * * * * *
            * * * * * * * *
           * * * * * * * * *
          * * * * * * * * * *
         * * * * * * * * * * *
        * * * * * * * * * * * *
       * * * * * * * * * * * * *



    Representation for the sum of the first 15, number(s)[ 105 ]

                    *
                   * *
                  * * *
                 * * * *
                * * * * *
               * * * * * *
              * * * * * * *
             * * * * * * * *
            * * * * * * * * *
           * * * * * * * * * *
          * * * * * * * * * * *
         * * * * * * * * * * * *
        * * * * * * * * * * * * *
       * * * * * * * * * * * * * *



    Representation for the sum of the first 16, number(s)[ 120 ]

                     *
                    * *
                   * * *
                  * * * *
                 * * * * *
                * * * * * *
               * * * * * * *
              * * * * * * * *
             * * * * * * * * *
            * * * * * * * * * *
           * * * * * * * * * * *
          * * * * * * * * * * * *
         * * * * * * * * * * * * *
        * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * *



    Representation for the sum of the first 17, number(s)[ 136 ]

                      *
                     * *
                    * * *
                   * * * *
                  * * * * *
                 * * * * * *
                * * * * * * *
               * * * * * * * *
              * * * * * * * * *
             * * * * * * * * * *
            * * * * * * * * * * *
           * * * * * * * * * * * *
          * * * * * * * * * * * * *
         * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * *



    Representation for the sum of the first 18, number(s)[ 153 ]

                       *
                      * *
                     * * *
                    * * * *
                   * * * * *
                  * * * * * *
                 * * * * * * *
                * * * * * * * *
               * * * * * * * * *
              * * * * * * * * * *
             * * * * * * * * * * *
            * * * * * * * * * * * *
           * * * * * * * * * * * * *
          * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 19, number(s)[ 171 ]

                        *
                       * *
                      * * *
                     * * * *
                    * * * * *
                   * * * * * *
                  * * * * * * *
                 * * * * * * * *
                * * * * * * * * *
               * * * * * * * * * *
              * * * * * * * * * * *
             * * * * * * * * * * * *
            * * * * * * * * * * * * *
           * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 20, number(s)[ 190 ]

                         *
                        * *
                       * * *
                      * * * *
                     * * * * *
                    * * * * * *
                   * * * * * * *
                  * * * * * * * *
                 * * * * * * * * *
                * * * * * * * * * *
               * * * * * * * * * * *
              * * * * * * * * * * * *
             * * * * * * * * * * * * *
            * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 21, number(s)[ 210 ]

                          *
                         * *
                        * * *
                       * * * *
                      * * * * *
                     * * * * * *
                    * * * * * * *
                   * * * * * * * *
                  * * * * * * * * *
                 * * * * * * * * * *
                * * * * * * * * * * *
               * * * * * * * * * * * *
              * * * * * * * * * * * * *
             * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 22, number(s)[ 231 ]

                           *
                          * *
                         * * *
                        * * * *
                       * * * * *
                      * * * * * *
                     * * * * * * *
                    * * * * * * * *
                   * * * * * * * * *
                  * * * * * * * * * *
                 * * * * * * * * * * *
                * * * * * * * * * * * *
               * * * * * * * * * * * * *
              * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 23, number(s)[ 253 ]

                            *
                           * *
                          * * *
                         * * * *
                        * * * * *
                       * * * * * *
                      * * * * * * *
                     * * * * * * * *
                    * * * * * * * * *
                   * * * * * * * * * *
                  * * * * * * * * * * *
                 * * * * * * * * * * * *
                * * * * * * * * * * * * *
               * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 24, number(s)[ 276 ]

                             *
                            * *
                           * * *
                          * * * *
                         * * * * *
                        * * * * * *
                       * * * * * * *
                      * * * * * * * *
                     * * * * * * * * *
                    * * * * * * * * * *
                   * * * * * * * * * * *
                  * * * * * * * * * * * *
                 * * * * * * * * * * * * *
                * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 25, number(s)[ 300 ]

                              *
                             * *
                            * * *
                           * * * *
                          * * * * *
                         * * * * * *
                        * * * * * * *
                       * * * * * * * *
                      * * * * * * * * *
                     * * * * * * * * * *
                    * * * * * * * * * * *
                   * * * * * * * * * * * *
                  * * * * * * * * * * * * *
                 * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 26, number(s)[ 325 ]

                               *
                              * *
                             * * *
                            * * * *
                           * * * * *
                          * * * * * *
                         * * * * * * *
                        * * * * * * * *
                       * * * * * * * * *
                      * * * * * * * * * *
                     * * * * * * * * * * *
                    * * * * * * * * * * * *
                   * * * * * * * * * * * * *
                  * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 27, number(s)[ 351 ]

                                *
                               * *
                              * * *
                             * * * *
                            * * * * *
                           * * * * * *
                          * * * * * * *
                         * * * * * * * *
                        * * * * * * * * *
                       * * * * * * * * * *
                      * * * * * * * * * * *
                     * * * * * * * * * * * *
                    * * * * * * * * * * * * *
                   * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 28, number(s)[ 378 ]

                                 *
                                * *
                               * * *
                              * * * *
                             * * * * *
                            * * * * * *
                           * * * * * * *
                          * * * * * * * *
                         * * * * * * * * *
                        * * * * * * * * * *
                       * * * * * * * * * * *
                      * * * * * * * * * * * *
                     * * * * * * * * * * * * *
                    * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 29, number(s)[ 406 ]

                                  *
                                 * *
                                * * *
                               * * * *
                              * * * * *
                             * * * * * *
                            * * * * * * *
                           * * * * * * * *
                          * * * * * * * * *
                         * * * * * * * * * *
                        * * * * * * * * * * *
                       * * * * * * * * * * * *
                      * * * * * * * * * * * * *
                     * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 30, number(s)[ 435 ]

                                   *
                                  * *
                                 * * *
                                * * * *
                               * * * * *
                              * * * * * *
                             * * * * * * *
                            * * * * * * * *
                           * * * * * * * * *
                          * * * * * * * * * *
                         * * * * * * * * * * *
                        * * * * * * * * * * * *
                       * * * * * * * * * * * * *
                      * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 31, number(s)[ 465 ]

                                    *
                                   * *
                                  * * *
                                 * * * *
                                * * * * *
                               * * * * * *
                              * * * * * * *
                             * * * * * * * *
                            * * * * * * * * *
                           * * * * * * * * * *
                          * * * * * * * * * * *
                         * * * * * * * * * * * *
                        * * * * * * * * * * * * *
                       * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 32, number(s)[ 496 ]

                                     *
                                    * *
                                   * * *
                                  * * * *
                                 * * * * *
                                * * * * * *
                               * * * * * * *
                              * * * * * * * *
                             * * * * * * * * *
                            * * * * * * * * * *
                           * * * * * * * * * * *
                          * * * * * * * * * * * *
                         * * * * * * * * * * * * *
                        * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 33, number(s)[ 528 ]

                                      *
                                     * *
                                    * * *
                                   * * * *
                                  * * * * *
                                 * * * * * *
                                * * * * * * *
                               * * * * * * * *
                              * * * * * * * * *
                             * * * * * * * * * *
                            * * * * * * * * * * *
                           * * * * * * * * * * * *
                          * * * * * * * * * * * * *
                         * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 34, number(s)[ 561 ]

                                       *
                                      * *
                                     * * *
                                    * * * *
                                   * * * * *
                                  * * * * * *
                                 * * * * * * *
                                * * * * * * * *
                               * * * * * * * * *
                              * * * * * * * * * *
                             * * * * * * * * * * *
                            * * * * * * * * * * * *
                           * * * * * * * * * * * * *
                          * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 35, number(s)[ 595 ]

                                        *
                                       * *
                                      * * *
                                     * * * *
                                    * * * * *
                                   * * * * * *
                                  * * * * * * *
                                 * * * * * * * *
                                * * * * * * * * *
                               * * * * * * * * * *
                              * * * * * * * * * * *
                             * * * * * * * * * * * *
                            * * * * * * * * * * * * *
                           * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 36, number(s)[ 630 ]

                                         *
                                        * *
                                       * * *
                                      * * * *
                                     * * * * *
                                    * * * * * *
                                   * * * * * * *
                                  * * * * * * * *
                                 * * * * * * * * *
                                * * * * * * * * * *
                               * * * * * * * * * * *
                              * * * * * * * * * * * *
                             * * * * * * * * * * * * *
                            * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 37, number(s)[ 666 ]

                                          *
                                         * *
                                        * * *
                                       * * * *
                                      * * * * *
                                     * * * * * *
                                    * * * * * * *
                                   * * * * * * * *
                                  * * * * * * * * *
                                 * * * * * * * * * *
                                * * * * * * * * * * *
                               * * * * * * * * * * * *
                              * * * * * * * * * * * * *
                             * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 38, number(s)[ 703 ]

                                           *
                                          * *
                                         * * *
                                        * * * *
                                       * * * * *
                                      * * * * * *
                                     * * * * * * *
                                    * * * * * * * *
                                   * * * * * * * * *
                                  * * * * * * * * * *
                                 * * * * * * * * * * *
                                * * * * * * * * * * * *
                               * * * * * * * * * * * * *
                              * * * * * * * * * * * * * *
                             * * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 39, number(s)[ 741 ]

                                            *
                                           * *
                                          * * *
                                         * * * *
                                        * * * * *
                                       * * * * * *
                                      * * * * * * *
                                     * * * * * * * *
                                    * * * * * * * * *
                                   * * * * * * * * * *
                                  * * * * * * * * * * *
                                 * * * * * * * * * * * *
                                * * * * * * * * * * * * *
                               * * * * * * * * * * * * * *
                              * * * * * * * * * * * * * * *
                             * * * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 40, number(s)[ 780 ]

                                             *
                                            * *
                                           * * *
                                          * * * *
                                         * * * * *
                                        * * * * * *
                                       * * * * * * *
                                      * * * * * * * *
                                     * * * * * * * * *
                                    * * * * * * * * * *
                                   * * * * * * * * * * *
                                  * * * * * * * * * * * *
                                 * * * * * * * * * * * * *
                                * * * * * * * * * * * * * *
                               * * * * * * * * * * * * * * *
                              * * * * * * * * * * * * * * * *
                             * * * * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 41, number(s)[ 820 ]

                                              *
                                             * *
                                            * * *
                                           * * * *
                                          * * * * *
                                         * * * * * *
                                        * * * * * * *
                                       * * * * * * * *
                                      * * * * * * * * *
                                     * * * * * * * * * *
                                    * * * * * * * * * * *
                                   * * * * * * * * * * * *
                                  * * * * * * * * * * * * *
                                 * * * * * * * * * * * * * *
                                * * * * * * * * * * * * * * *
                               * * * * * * * * * * * * * * * *
                              * * * * * * * * * * * * * * * * *
                             * * * * * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 42, number(s)[ 861 ]

                                               *
                                              * *
                                             * * *
                                            * * * *
                                           * * * * *
                                          * * * * * *
                                         * * * * * * *
                                        * * * * * * * *
                                       * * * * * * * * *
                                      * * * * * * * * * *
                                     * * * * * * * * * * *
                                    * * * * * * * * * * * *
                                   * * * * * * * * * * * * *
                                  * * * * * * * * * * * * * *
                                 * * * * * * * * * * * * * * *
                                * * * * * * * * * * * * * * * *
                               * * * * * * * * * * * * * * * * *
                              * * * * * * * * * * * * * * * * * *
                             * * * * * * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 43, number(s)[ 903 ]

                                                *
                                               * *
                                              * * *
                                             * * * *
                                            * * * * *
                                           * * * * * *
                                          * * * * * * *
                                         * * * * * * * *
                                        * * * * * * * * *
                                       * * * * * * * * * *
                                      * * * * * * * * * * *
                                     * * * * * * * * * * * *
                                    * * * * * * * * * * * * *
                                   * * * * * * * * * * * * * *
                                  * * * * * * * * * * * * * * *
                                 * * * * * * * * * * * * * * * *
                                * * * * * * * * * * * * * * * * *
                               * * * * * * * * * * * * * * * * * *
                              * * * * * * * * * * * * * * * * * * *
                             * * * * * * * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 44, number(s)[ 946 ]

                                                 *
                                                * *
                                               * * *
                                              * * * *
                                             * * * * *
                                            * * * * * *
                                           * * * * * * *
                                          * * * * * * * *
                                         * * * * * * * * *
                                        * * * * * * * * * *
                                       * * * * * * * * * * *
                                      * * * * * * * * * * * *
                                     * * * * * * * * * * * * *
                                    * * * * * * * * * * * * * *
                                   * * * * * * * * * * * * * * *
                                  * * * * * * * * * * * * * * * *
                                 * * * * * * * * * * * * * * * * *
                                * * * * * * * * * * * * * * * * * *
                               * * * * * * * * * * * * * * * * * * *
                              * * * * * * * * * * * * * * * * * * * *
                             * * * * * * * * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 45, number(s)[ 990 ]

                                                  *
                                                 * *
                                                * * *
                                               * * * *
                                              * * * * *
                                             * * * * * *
                                            * * * * * * *
                                           * * * * * * * *
                                          * * * * * * * * *
                                         * * * * * * * * * *
                                        * * * * * * * * * * *
                                       * * * * * * * * * * * *
                                      * * * * * * * * * * * * *
                                     * * * * * * * * * * * * * *
                                    * * * * * * * * * * * * * * *
                                   * * * * * * * * * * * * * * * *
                                  * * * * * * * * * * * * * * * * *
                                 * * * * * * * * * * * * * * * * * *
                                * * * * * * * * * * * * * * * * * * *
                               * * * * * * * * * * * * * * * * * * * *
                              * * * * * * * * * * * * * * * * * * * * *
                             * * * * * * * * * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 46, number(s)[ 1035 ]

                                                   *
                                                  * *
                                                 * * *
                                                * * * *
                                               * * * * *
                                              * * * * * *
                                             * * * * * * *
                                            * * * * * * * *
                                           * * * * * * * * *
                                          * * * * * * * * * *
                                         * * * * * * * * * * *
                                        * * * * * * * * * * * *
                                       * * * * * * * * * * * * *
                                      * * * * * * * * * * * * * *
                                     * * * * * * * * * * * * * * *
                                    * * * * * * * * * * * * * * * *
                                   * * * * * * * * * * * * * * * * *
                                  * * * * * * * * * * * * * * * * * *
                                 * * * * * * * * * * * * * * * * * * *
                                * * * * * * * * * * * * * * * * * * * *
                               * * * * * * * * * * * * * * * * * * * * *
                              * * * * * * * * * * * * * * * * * * * * * *
                             * * * * * * * * * * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 47, number(s)[ 1081 ]

                                                    *
                                                   * *
                                                  * * *
                                                 * * * *
                                                * * * * *
                                               * * * * * *
                                              * * * * * * *
                                             * * * * * * * *
                                            * * * * * * * * *
                                           * * * * * * * * * *
                                          * * * * * * * * * * *
                                         * * * * * * * * * * * *
                                        * * * * * * * * * * * * *
                                       * * * * * * * * * * * * * *
                                      * * * * * * * * * * * * * * *
                                     * * * * * * * * * * * * * * * *
                                    * * * * * * * * * * * * * * * * *
                                   * * * * * * * * * * * * * * * * * *
                                  * * * * * * * * * * * * * * * * * * *
                                 * * * * * * * * * * * * * * * * * * * *
                                * * * * * * * * * * * * * * * * * * * * *
                               * * * * * * * * * * * * * * * * * * * * * *
                              * * * * * * * * * * * * * * * * * * * * * * *
                             * * * * * * * * * * * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *



    Representation for the sum of the first 48, number(s)[ 1128 ]

                                                     *
                                                    * *
                                                   * * *
                                                  * * * *
                                                 * * * * *
                                                * * * * * *
                                               * * * * * * *
                                              * * * * * * * *
                                             * * * * * * * * *
                                            * * * * * * * * * *
                                           * * * * * * * * * * *
                                          * * * * * * * * * * * *
                                         * * * * * * * * * * * * *
                                        * * * * * * * * * * * * * *
                                       * * * * * * * * * * * * * * *
                                      * * * * * * * * * * * * * * * *
                                     * * * * * * * * * * * * * * * * *
                                    * * * * * * * * * * * * * * * * * *
                                   * * * * * * * * * * * * * * * * * * *
                                  * * * * * * * * * * * * * * * * * * * *
                                 * * * * * * * * * * * * * * * * * * * * *
                                * * * * * * * * * * * * * * * * * * * * * *
                               * * * * * * * * * * * * * * * * * * * * * * *
                              * * * * * * * * * * * * * * * * * * * * * * * *
                             * * * * * * * * * * * * * * * * * * * * * * * * *
                            * * * * * * * * * * * * * * * * * * * * * * * * * *
                           * * * * * * * * * * * * * * * * * * * * * * * * * * *
                          * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                         * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                      * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                     * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                    * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                   * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                  * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                 * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
                * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
               * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
              * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
             * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
            * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
           * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
          * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
         * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
        * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *
       * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *


<a id="org1009e63"></a>

# Conclusion

As shown above, numbers, in concert with operations like addition,
can be configured to assume interesting geometric shapes. More
interesting shapes in higher dimensions like cubes can be obtained
from such simple operations on numbers.

In general, such numbers that are obtained from adding classes of
other numbers and arriving at interesting geometric shapes are
called polygonal numbers.
