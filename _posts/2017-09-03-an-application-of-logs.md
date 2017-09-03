---
layout: post
title: Python's dynamic type system!
publish: true
---

# On one application of logarithms

Logarithms play an essential role in numerical computations. First, what are
they?

If you multiply a number 1 time by itself, you obtain a power of that number.
Typically \[ 2 * 2 = 2^2 \].

From this it follows that if you multiply a number, \[ x\], by itself, \[ n \] times, you
obtain the power \[ x ^ n \].

The number \[ x \] is called the base or root and the number \[ n \] is called the exponent.
Together, \[ x ^ n \] is called a power. It's also very important to name results of
operations, hence, let's call the result of raising \[ x \] to the \[ n \]th
power, \[ y \].

This implies that, \[ x ^ n = y \]. The number \[ y \] can now be seen as the
power \[x ^ n \], by virtue of equality. A
practical example is \[ 2^3 \], which is \[8\]. The investigator is always busy searching
for an unkown. Suppose we are given an incomplete power and demanded to analyse
it and determine the unkown. Suppose instead of stating that \[ 2 ^ 3 \] is \[ 8
\], we are
asked the question: what is \[ 2 ^ 3 \]?

The response is easy, we say, \[ 2^3 = 8 \].

What if we are asked, what is the exponent \[ x \], such that \[ 2 \] raised to
\[ x \] would
yield \[ 8 \]. That is if \[ 2^x = 8 \], what is the value of \[ x \] ?

The algebraist would say, \[ x \] is \[ 3 \]. The number \[ 8 \] can be
expressed as \[ 2^3 \]. Hence,
the relation above can be written as \[ 2^x = 2^3 \]. The number \[ 8 \] has been replaced
by its equivalent \[ 2^3 \]. Comparing both sides, we gain the insight that the left hand
side can be resolved to \[ 8 \] by substituting \[3 \] for \[ x \]. Therefore,
\[ x = 3\], and that's the result.

The word lograrithm can be taken to mean the synonym for exponent. We'll see
how. Suppose we are given the power \[ 2^3 \] and are asked to name its parts.
We'll say: \[ 2\] is the root, and \[ 3 \] is the exponent. 

The logarithm of the power \[ 2^3 \] is 3. Don't ask me how. However, the
logarithm of a power or a number, is the exponent to which the root or the
number must be raised in order to get the result(require 'ob-python)
(org-babel-do-load-languages
 'org-babel-load-languages
 '((python . t)))
ing value represented by the
power. Interestingly, that number is also called the exponent. 

It follows that the logarithm of \[ 2 ^ 3 \] is \[ 3 \]. 

To generalize this, let log stand for logarithm and it will follow from this
that \[ \log(x ^ n) = n \]. 

Also, \[ x ^ n = y \] ,hence, \[ \log(x^n) = \log(y) = n \].

Summarily, in the whole spectrum of numbers, every integer can be represented as
a logarithm. The logarithm of any integer can be expressed as a decimal
fraction. Since, our natural base for arithmetic is base 10, every integer can
be expressed as a logarithm in the base of 10.

Let's investigate further. The question will be, what number can we raise \[ 10 \] to,
in order to obtain \[ 10 \] itself. The answer is \[ 1\]. The number \[ 10 \]
raised to the power \[ 1 \] is \[ 10 \]. Hence, \[ \log(10^1) = 10 \].
Logarithms are not defined for negative numbers, and this throws some light on
the development of logarithms of numbers in base 10. 

Precisely, we can ask the question, how does the logarithm behave for numbers
greater than \[ 0 \], but less than \[ 10 \]  and how does it behave for numbers
greater than \[ 10 \]. We know that \[ \log(10) = 1 \]. Hence, the logarithms of
numbers less than \[ 10 \] should be less than 1, and the logarithms of numbers
greater than 10 should be greater than \[ 1 \]. Similarly, numbers less than \[
10 \] have single digits and numbers greater than \[ 10 \]  have multiple
digits. 

Back to the assertion that logarithms can be expressed using decimal fractions.
Decimal fractions often have 2 parts: an integral part which appears before the
\[ . \], and the fractional part which appears after. The integral part of a
decimal fraction in the case of logarithms is called its *characteristic*. It is
this *characteristic* which will show us one beautiful application of
logarithms.

\[ \log(1) = 0 \]
\[ \log(2) = 0.30102999566 \]

The characteristic is \[ \log(2) is 0 \]

Hence, we know and we can see that all the numbers less than \[ 10 \] will have
a characteristic of \[ 0 \]. And we can conclude that every single digit number
has a characteristic of \[ 0 \]. We can further conclude that a characteristic
of \[ 0 \] implies that a number in question is single-digit. 

How about numbers greater than \[ 10? \]

\[ \log (12) = 1.07918124605 \]
\[ \log (99) = 1.9956351946 \]
\[ \log (123) = 2.08990511144 \]
\[ \log (321) = 2.5065050324 \]

So far, single digit numbers have a characteristic of 0, double digit numbers
have a characteristic of 1, and triple digit numbers have a characteristic of 2. 

Is there a pattern in this development? 

Let's test for numbers with quadruple, quintuple, sextuple and septuple digits.

\[ \log(1234) = 3.0913151597 \], 4 digits with a characteristic of 3.
\[ \log(12345) = 4.09149109427 \], 5 digits with a characteristic of 4.
\[ \log(123456) = 5.09151220163 \], 6 digits with a characteristic of 5.
\[ \log(1234567) = 6.09151466409 \], 7 digits with a characteristic of 6.

The pattern is, an [\\ n \\]-th digit has a characteristic  of \[ n - 1 \]. And we
can also state that: a characteristic of \[ n \]  asserts that the integer in
question has \[ n + 1 \] digits.

Now, what is the application of this finding?

Well, it's easy. Logarithms can be used to find the number of digits of a given
integer. It may be wise to take the absolute value of integers in performing
such operations since logarithms are undefined for negative numbers, but
negative integers also have a number of digits.

This finding becomes very essential in computer programming. One can, therefore,
write a program that computes the length of digits of an integer by computing
the logarithm, taking the characteristic of the result and adding \[ 1 \] to it.


<a id="org62853ae"></a>

## Simple algorithm for computing the length of an integer

1.  Get number; if number is not an integer, exit
2.  Compute the logarithm of the number
3.  Extract the digit before the decimal point, that is the characteristic
4.  Add one to this value
5.  Return the sum

The sum returned will be the length of digits in the given number. I'd say that
one can simply take the result of flooring the logarithm of the given number. 

Below is a python program that computes the length of digits of its integral
arguments. 

    import math
    """
    numDigits receives an integer as an argument and returns the number of digits it has.
    It computes the length of digits using logs, and int function to extract the integral part.
    For each input, it obtains its absolute value, then it computes the log, and returns the integral part of the result
    """
    def numDigits(n):
        num = abs(n)
        num_log = math.log(num, 10)
        num = int(num_log) + 1
        
        return num
    
    # now let's run a few examples
    for i in range (10):
        n = (i + 1) * (10 ** i)
        print "%d has %d digits" % (n, numDigits(n))

    1 has 1 digits
    20 has 2 digits
    300 has 3 digits
    4000 has 4 digits
    50000 has 5 digits
    600000 has 6 digits
    7000000 has 7 digits
    80000000 has 8 digits
    900000000 has 9 digits
    10000000000 has 11 digits

And that is an application of logarithms.

Now that we are, we can show the other method for computing the another
technique for computing the length of digits of a given number. This method
relies on successive integer divisions and subsequent manipulation of
remainders. 

    import math
    """
    numDigits2 receives an integer as an argument and returns the number of digits it has.
    It computes the length of digits by recursively counting the digits
    """
    def numDigits2(n):
        num = abs(n)
        
        if num < 10:
            return 1
    
        num = num // 10
        return 1 + numDigits2(num)
    
    # now let's run a few examples
    for i in range (10):
        n = (i + 1) * (10 ** i)
        print "%d has %d digits" % (n, numDigits2(n))

    1 has 1 digits
    20 has 2 digits
    300 has 3 digits
    4000 has 4 digits
    50000 has 5 digitsy
    600000 has 6 digits
    7000000 has 7 digits
    80000000 has 8 digits
    900000000 has 9 digits
    10000000000 has 11 digits

And that's that. You can compare, at leisure, the efficiency of each of the
methods.

Thanks for reading.

