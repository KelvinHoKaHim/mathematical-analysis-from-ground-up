---
title: [The Real Number \#01] Pythagoras and the Myth of Rational Number
date: 2025-06-25 +0800
categories: [Analysis of Onc variable, The Real Number]
tags: [mathematical-analysis, real-number, Pythagoras, Pythagoras's-theorem, rational-number]     # TAG names should always be lowercase
---

## Pythagoras Theorem Exposes Fault of the Rational Numbers
The Pythagorean theorem was well-known in many ancient cultures, including the Babylonians and Indians, but it was the Greeks who first provided a proof, to which its discovery was often attributed to the Pythagorean school.

<b>Theorem 1. (Pythagoras' Theorem)</b> <i>In a right triangle, the square of the length of the hypotenuse is equal to the sum of the squares of the lengths of the other two sides.
$$
a^2 + b^2 = c^2
$$
where $c$ is the length of the hypotenuse and $a$ and $b$ are the lengths of the other two sides.</i>

<i>Proof.</i><br>&#x25A1;

The Pythagorean theorem prompted the discovery of irrational numbers. Consider a right triangle with both legs of length $1$. By the Pythagorean theorem, the length of the hypotenuse is $\sqrt{2}$. However, it can be proved that $\sqrt{2}$ is not a could never be represented as the ratio of two integers, which can be found in Euclide's <i>Element</i>.

<b>Lemma 1. (Euclid's lemma)</b> <i>Let $p,m,n\in\Z$, where $p$ is a prime number. Suppose $p\mid mn$. Then $p|m$ or $p|n$.</i>

<i>Proof.</i> Omitted.<br>&#x25A1;

<b>Remark 1.</b> The original proof from the \textit{Element} is convoluted and difficult. Modern proof of the lemma often involves Bezout's lemma, which states that for any integer $a,b$, if they are coprime ($\text{gcd}(a,b) =1$), then there is integer $s,t\in\Z$ such that $as + bt = 1$. To provide a rigorous proof from both ways would distract us to a lengthy detour. Interested reader can consult the <i>>Elements</i> or any introductory textbook on number theory.

<b>Theorem 2.</b> <i>The number $\sqrt{2}$ is irrational.</i>

<i>Proof.</i> Suppose $\sqrt{2}$ is rational, then there is $m,n\in\Z$. where $\text{gcd}(m,n) = 1$, such that $\sqrt{2} = m/n$ , which means $m^2 = 2n^2$. Since $2|m^2$, Euclid's lemma implies that $2|m$. Then there is some $k\in\Z$ such that $m = 2k$. Substituting this equation to $m^2 = 2n^2$, we have $2k^2 = n^2$. Applying Euclid's lemma again, we have $2|n$. This contradicts the assumption that $\text{gcd}(m,n) = 1$. Therefore, $\sqrt{2}$ is irrational.<br>&#x25A1;

This fact shows that the rational numbers is <i>incomplete</i>, in the sense that not all quantity can be represented by a rational numbers. There are many "holes" in the rational line. 
Hence, we need to define a larger system of numbers to fill in these holes----the set of real numbers $\R$.

In the next few section, we will try to achieve the following thing: 
1. Identify the defining properties of the real numbers.
2. Study the properties of the real number
3. Demonstrate why the properties uniquely pick out a certain structure.
4. Prove that such a structure do indeed exists.


## Real Numbers is Ordered
