---
title: "Proving Bernoulli’s Sum of Powers"
source: https://towardsdatascience.com/proving-bernoullis-sum-of-powers-22f50df188e9
clipped: 2023-10-12
tags: []
---

## How to Calculate the Sum of the p Powers of the n First Integers

Among his many significant contributions, the renowned Swiss mathematician [Jacob Bernoulli](https://en.wikipedia.org/wiki/Jacob_Bernoulli) (1655–1705), one of the many notable mathematicians in [his family](https://en.wikipedia.org/wiki/Bernoulli_family) (the Bernoulli family gave origin to a total of eight world-famous mathematicians) provided, in 1713, an expression for the sum of the *p* powers of the *n* first integers (which he called [Summae Potestatum](https://en.wikipedia.org/wiki/Faulhaber%27s_formula#Summae_Potestatum)). His solution, which has the form of a [polynomial function](https://en.wikipedia.org/wiki/Polynomial#Polynomial_functions) of *n* of degree (*p* \+ 1), contains coefficients involving the ubiquitous and now famous [Bernoulli numbers](https://en.wikipedia.org/wiki/Bernoulli_number) (a sequence of fractional numbers which occur in numerous areas of both mathematics and theoretical physics).

[

![](https://miro.medium.com/v2/resize:fit:700/1*b6ty5hQOLdMGBdQvMnXx0w@2x.png)

](https://en.wikipedia.org/wiki/Faulhaber's_formula#Summae_Potestatum)

Figure 1: In 1713, the prominent Swiss mathematician Jacob Bernoulli ([source](https://en.wikipedia.org/wiki/Jacob_Bernoulli)), published the *Summae Potestatum,* an expression for the sum of the *p* powers of the *n* first integers ([source](https://en.wikipedia.org/wiki/Faulhaber%27s_formula)).

The sum, known as [Faulhaber’s formula](https://en.wikipedia.org/wiki/Faulhaber%27s_formula) (named after the German mathematician [Johann Faulhaber](https://en.wikipedia.org/wiki/Johann_Faulhaber) (1580–1635)), whose result Bernoulli published under the title [Summae Potestatum](https://en.wikipedia.org/wiki/Faulhaber%27s_formula#Summae_Potestatum)*,* is given by the following expression

![](https://miro.medium.com/v2/resize:fit:700/1*IpkOMIoN4sEhcNsvF4--kA@2x.png)

Equation 1: The sum of the *p*\-th powers of the first *n* positive integers, known as [Faulhaber’s formula](https://en.wikipedia.org/wiki/Faulhaber%27s_formula).

![](https://miro.medium.com/v2/resize:fit:556/1*rtiDp4VIOniFwJydPUrZcg@2x.png)

Figure 2: The German mathematician Johann Faulhaber (1580–1635). Faulhaber was a polymath, who was trained as a weaver, worked on the fortifications of several cities, built water wheels and geometrical instruments for the military, among other things ([source](https://en.wikipedia.org/wiki/Johann_Faulhaber)).

As noted by [these exceptional lectures on number theory](https://people.reed.edu/~jerry/) the calculation becomes much tidier if one writes the sum starting at the index *m*\=0 and ending at the index *m* = *n*\-1. With this alternative choice of indexes, the sum becomes:

![](https://miro.medium.com/v2/resize:fit:700/1*j7aB0DMvv5XxT4lGufAQmg@2x.png)

Equation 2: Eq. 1 written with the sum starting at the index *m*\=0 zero and ending at the index *m* = *n*\-1. Choosing this new set of indexes “neatens” the calculations.

Now consider the so-called [generating function](https://en.wikipedia.org/wiki/Generating_function) **S**(*n*,*t*), a [power series](https://en.wikipedia.org/wiki/Power_series) that has the sums in Eqs. 1 and 2 as coefficients:

![](https://miro.medium.com/v2/resize:fit:420/1*09wsGv1japtLTRIIsQiOTA@2x.png)

Equation 3: The generating function has the sums given by Eqs. 1 and 2 as coefficients. According to [Wikipedia](https://en.wikipedia.org/wiki/Generating_function), a generating function “is a way of encoding an infinite sequence of numbers by treating them as the coefficients of a power series”.

Substituting Eq. 2 in Eq. 3 we get the double sum:

![](https://miro.medium.com/v2/resize:fit:389/1*7zm7BdVo764RHeucz0gGVw@2x.png)

Equation 4: Eq. 3 after the substituting of Eq. 2.

where *k* is an integer number. After a few steps of algebra used to rearrange the sums, we can re-express Eq. 4 by the following product of two functions:

![](https://miro.medium.com/v2/resize:fit:383/1*3wP20Zrq4UFA2HdNxePNtg@2x.png)

Equation 5: Eq. 4 rewritten as a product of two functions. This expression is obtained after rearranging the sums and performing some simple (but not very illuminating) algebraic manipulations.

Eq. 5 is obtained by rearranging the double sum in Eq. 4 and performing some simple (but not very illuminating) algebraic manipulations. Now, the first factor of **S**(*n*,*t*) can be trivially written as a power series using the Taylor expansion of the exponential function:

![](https://miro.medium.com/v2/resize:fit:660/1*cbRriV0bpTJ1dqJpOUBoOQ@2x.png)

Equation 6: The power series expansion of the exponential function.

(you just have to subtract 1 from the left-hand side of Eq. 6 and divide both sides by *x*). To write the second term of **S**(*n*,*t*) one has to introduce the previously mentioned [Bernoulli numbers](https://en.wikipedia.org/wiki/Bernoulli_number). The function *t*/(e*ᵗ*\-1) in Eq. 5 becomes:

![](https://miro.medium.com/v2/resize:fit:320/1*3iR_rpfwFO2S8m12T4OyUg@2x.png)

Equation 7: In order to write the second factor of **S**(*n*,*t*) in Eq. 5 one introduces the Bernoulli numbers.

Skipping a few steps (to avoid cluttering), the generating function **S**(*n*,*t*) becomes the following intricate expression:

![](https://miro.medium.com/v2/resize:fit:700/1*L2QyWFfqVWx-s5_1_a5LGA@2x.png)

Equation 8: The generating function given originally by Eq. 3 after using the exponential function time series and Eq. 7 (which contains Bernoulli numbers).

Now, the next step is to define the so-called [Bernoulli polynomials](https://en.wikipedia.org/wiki/Bernoulli_polynomials):

![](https://miro.medium.com/v2/resize:fit:447/1*aRtuoSa3WbNWNy-ilkK9FA@2x.png)

Equation 9: Definition of the Bernoulli polynomials shown in Fig. 3 below.

The figure below shows several examples of Bernoulli polynomials corresponding to different values of Bernoulli numbers.

![](https://miro.medium.com/v2/resize:fit:700/1*9MzujcIGrxJgJZYEyPcFxA@2x.png)

Figure 3: The Bernoulli polynomials for several values of the Bernoulli numbers ([source](https://en.wikipedia.org/wiki/Bernoulli_polynomials)).

Comparing the original expression for the generating function **S**(*n*,*t*) with Eq. 8 and using the definition of Bernoulli polynomials, we obtain:

![](https://miro.medium.com/v2/resize:fit:527/1*1rd1kQT5lUXeR8QNHCguHQ@2x.png)

Equation 10: Final expression for the sum of the *p* powers of the *n* first integers that we are after.

Note that the generating function can be elegantly written as:

![](https://miro.medium.com/v2/resize:fit:700/1*RGVvUjeAzmgBlHIBKne7zg@2x.png)

Equation 11: The final expression for the generating function, expressed in terms of Bernoulli polynomials and Bernoulli numbers.

In a [previous article](https://towardsdatascience.com/on-the-sums-of-series-of-reciprocals-6711437ad893) (see below) I derived the first five Bernoulli numbers. They are given by:

![](https://miro.medium.com/v2/resize:fit:700/1*edYTRF8RBqHg1IRDx9QDAQ@2x.png)

Equation 12: The first five Bernoulli numbers derived in [this article](https://towardsdatascience.com/on-the-sums-of-series-of-reciprocals-6711437ad893).

![](https://miro.medium.com/v2/resize:fit:700/1*aWQ6zSByw2mkhYjziCY70A@2x.png)

Figure 4: On the left, the Japanese mathematician Kowa Seki. On the right, a page from his work *Katsuyo Sampo (1712), where he* tabulates binomial coefficients and Bernoulli numbers.

Using Eq. 9 we obtain some Bernoulli polynomials (see Fig. 3):

![](https://miro.medium.com/v2/resize:fit:700/1*SGjUeDqmkenT4EYqAzQDtA@2x.png)

Equation 13: The first Bernoulli polynomials.

Now we have all the tools we need! The following are two simple examples of the sum we are after, but all other cases can be trivially obtained:

![](https://miro.medium.com/v2/resize:fit:700/1*enHFl0qUPbrPPuW1AK4otg@2x.png)

Equation 14: Two simple examples of sums of the *p* powers of the *n* first integers.