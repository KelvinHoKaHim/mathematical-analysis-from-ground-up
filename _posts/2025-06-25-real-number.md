---
title: Real Analysis 01 | The Inception of Real Number
date: 2025-06-25 +0800
categories: [01 Real Analysis of One Variable, The Real Number]
tags: [mathematical-analysis, real-number, Pythagoras, Pythagoras's-theorem, rational-number]     
math: true
---

## Numbers and Commensurability

Human's discovery of the real number is indeed a remarkable feat. The flowing of time, the height of a tree, the speed of a horse, etc. are all phenomena distinct and independent to one another. There are no reasons to expect these phenomena could be described with the same number system. But we nonetheless discovered they can all be modeled and describe using real numbers.

Given how pervasive the structure of real number is in our lived experienced, it seems fruitful to study this structure in isolation. So that even when we encounter phenomena that are entirely fresh to us, we can still make reasonable predictions to their development.

The Greeks approached their study of the real number from Geometry. Greek mathematician, who only knew the natural numbers at that time, considered how could one measure the length of two objects. Suppose we have two wooden sticks of different length, how should we describe their difference in length? That would require a common unit that we apply on the two sticks, and then the length of the sticks would be described as a integer multiple of that unit. 

But this method of measurement assumed that for any two length, there exists a common unit that can express the two lengths as integer multiple of the common unit. This is indeed the assumption of the Greek, who call such a property <i>Commeasurability</i>.

Suppose that we have two stick $A$ and $B$, each with length $5$ units and $2$ units. We can describe the length of $A$ with the length of $B$ without explicitly referring to their common unit. which to express the relation of their length as ratios. In our case, the length of $A$ and $B$ has a ratio of $5:2$. Then, to find the length of $A$ given $B$, we can divide $B$ into two parts, then add up the length of that part five times. The resultant length of be equivalent to that of $A$. 

Putting all those cumbersome terminologies aside, this is basically saying that the relation of the length of $A$ and length of $B$ can be expressed as

$$
length_A = \frac{5}{2} \times length_B
$$

Hence, it seemed that any length could either be desribed by a integer multiple of a certain unit, or a ratio between another length.

![two-sticks](image/2025-06-25-real-number-01.jpg){: w="700"}
_Comparing the length of two sticks._
## Pythagoras Theorem Exposes Fault of the Rational Numbers

The Pythagorean theorem was well-known in many ancient cultures, including the Babylonians and Indians, but it was the Greeks who first provided a proof, to which its discovery was often attributed to the Pythagorean school.

<b>Theorem 1. (Pythagoras' Theorem)</b> <i>In a right triangle, the square of the length of the hypotenuse is equal to the sum of the squares of the lengths of the other two sides.
$$
a^2 + b^2 = c^2
$$
where $c$ is the length of the hypotenuse and $a$ and $b$ are the lengths of the other two sides.</i>

<i>Proof.</i><br>&#x25A1;

The Pythagorean theorem prompted the discovery of irrational numbers. Consider a right triangle with both legs of length $1$ unit. By the Pythagorean theorem, the length of the hypotenuse is $\sqrt{2}$ unit. However, it can be proved that $\sqrt{2}$ is not a could never be represented as the ratio of two integers, which can be found in Euclid's <i>Element</i>.

<b>Lemma 1. (Euclid's lemma)</b> <i>Let $p,m,n\in\mathbb{Z}$, where $p$ is a prime number. Suppose $p\mid mn$. Then $p|m$ or $p|n$.</i>

<i>Proof.</i> Omitted.<br>&#x25A1;

<b>Remark 1.</b> The original proof from the <i>Element</i> is convoluted and difficult. Modern proof of the lemma often involves Bezout's lemma, which states that for any integer $a,b$, if they are coprime ($\text{gcd}(a,b) =1$), then there is integer $s,t\in\mathbb{Z}$ such that $as + bt = 1$. To provide a rigorous proof from both ways would distract us to a lengthy detour. Interested reader can consult the <i>>Elements</i> or any introductory textbook on number theory.

<b>Theorem 2.</b> <i>The number $\sqrt{2}$ is irrational.</i>

<i>Proof.</i> Suppose $\sqrt{2}$ is rational, then there is $m,n\in\mathbb{Z}$. where $\text{gcd}(m,n) = 1$, such that $\sqrt{2} = m/n$ , which means $m^2 = 2n^2$. Since $2\mid m^2$, Euclid's lemma implies that $2\mid m$. Then there is some $k\in\mathbb{Z}$ such that $m = 2k$. Substituting this equation to $m^2 = 2n^2$, we have $2k^2 = n^2$. Applying Euclid's lemma again, we have $2\mid n$. This contradicts the assumption that $\text{gcd}(m,n) = 1$. Therefore, $\sqrt{2}$ is irrational.<br>&#x25A1;

This fact shows that the rational numbers is <i>incomplete</i>, in the sense that not all quantity can be represented by a rational numbers. There are many "holes" in the rational line. 
Hence, we need to define a larger system of numbers to fill in these holes----the set of real numbers $\mathbb{R}$.

![hole-in-real-number](image/2025-06-25-real-number-02.jpg){: w="700"}
_There are many "holes" in the rational line. The hole at $\sqrt{2}$ is one of them._

In the next few section, we will try to achieve the following thing: 
1. Identify the defining properties of the real numbers.
2. Study the properties of the real number
3. Demonstrate why the properties uniquely pick out a certain structure.
4. Prove that such a structure do indeed exists.

![hierarchy-of-numbers](image/2025-06-25-real-number-03.jpg){: w="700"}
_The hierarchy of numbers._

## Real Numbers is Ordered
