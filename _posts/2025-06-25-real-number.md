---
title: Real Analysis 01 | The Inception of Real Number
date: 2025-06-25 +0800
categories: [01 Real Analysis of One Variable, The Real Number]
tags: [real-analysis, real-number, Pythagoras, Pythagoras's-theorem, rational-number, Aristotle, Dedekind-cut]     
math: true 
---

## Aristotle's Conception of Continuity

Our understanding of time, space, and motion is inseparable from the notion of continuity. The flowing of the seconds, the extension of a table, and the movement of a horse, all seemed to be carried out in a continuous fashion. There seems to never be gaps between two moments, nor there are any gaps on a continuous piece of wood. In his <i>Physics</i>, Aristotle provide two characterisation of continuity:
1. Things are called continuous when the touching limits of each become one and the same and are, as the word implies, contained in each other (V, 3);
2. Everything continuous is divisible into divisibles that are infinitely divisible (VI, 1)

The first characterisation could be rendered as a two place relation. A and B are continuous if their extremities touch in a way such that they share the same extremity. And as a consequence of being continous, A and B are parts of the same continuous whole. While, the second characterisation simply states that a continous objects can be divided infinitely without end. 

As a consequent of such characterisation, Aristotle argued that a continuous extent could not be composed of indivisible points, i.e. atom. Aristotle has three arguments, I will only present two here, which I find more interesting (VI, 1).

<i>First argument</i>
1. If a continuous line is composed of points, then there are distinct points A and B that A and B must have their extremities in contact (Characterisation 1)
2. If two things are in contact, then either 

    - part of one is in contant with part of another, 

    - part of one is in contact with the whole of another, or 

    - the whole of one is in contact with the whole of another. 

3. A and B have no parts. (Definition of indivisibility)
4. From 2 and 3, the whole of A is in contact with the whole of B.
5. For two things to be spacially separated, some parts of one thing should occupy space parts of the other do not.
5. From 4 and 5, A and B are not spacially separated
6. Since A and B are not spacially separable, they are not distinct. This leads to a contradiction.


<i>Second argument.</i>

1. If A and B are dinctint indivisible points that are continuous, then they are in succession (i.e. being next to another).
2. If two things are in succession, then nothing are between the two things.
3. From 1 and 2, nothing is between A and B.
4. Since A and B are distinct points, a line can be drawn to connect A and B.
5. For any line, a point can be found on the line that is not an extremity.
6. From 4,5 there is a point between A and B. A contradiction arises.

From these considerations, Aristotle concluded that a continuous things can never be composed of atoms. We will see whether these ideas are defeasible as we develop our account of real numbers.

There is a point that needs to be addressed before we proceed any further. Attentive reader may raise that extended objects in reality are truly not continuous--they are made up of truly indivisible parts, i.e. subatomic particles. But let's just set our prior metaphysical knowledge of the world aside for a moment, and focus on how phenomena of extended objects are presented to us, we will find they are always accompanied by the <i>appearance of continuity</i>, irregardless of whether they are truly continuous or not. Now this structure of continuity is what we are really interested in studying. 

## Measurement and Commesurability

It is difficult to study the notion of "continuity" along without reference to real life instances of continuity such as the breath of a rod. To connect the abstract world of mathematics with real occurence, we need the art of <i>measurement</i> 

Greek mathematician, who had a sharp distinction between the discrete and the continuous. Did not conceived of numbers as a measure of continuous magnitude. Numbers, for all they knew, only referred to natural numbers. They are nothing but measure of discrete quantities. But without numbers, how could we describe the length of an extended object? The answer was adopting a suitable unit.

Given two iron rods of different length, how should we describe their difference in length? That would require a common unit that we apply on the two rods, and then the length of the rods would be described as an integer multiple of that unit. 


Suppose that we have two rods $A$ and $B$, each with length $5$ units and $2$ units. We can describe the length of $A$ with the length of $B$ without explicitly referring to their common unit. which to express the relation of their length as ratios. In our case, the length of $A$ and $B$ has a ratio of $5:2$. Then, to find the length of $A$ given $B$, we can divide $B$ into two parts, then add up the length of that part five times. The resultant length of be equivalent to that of $A$. 

Putting all those cumbersome terminologies aside, this is basically saying that the relation of the length of $A$ and length of $B$ can be expressed as

$$
length_A : length_B = 5:2
$$

Hence, it seemed that any length could either be described by an integer multiple of a certain unit, or a ratio between another length.

But this method of measurement assumed that for any two length, there exists a common unit that can express the two lengths as integer multiple of the common unit. This is indeed the assumption of the Greek, who call such a property <i>Commeasurability</i>.

![two-rods](image/2025-06-25-real-number-01.jpg){: w="700"}
_Comparing the length of two rods._
## Pythagoras Theorem Exposes Fault of the Rational Numbers

The Pythagorean theorem was well-known in many ancient cultures, including the Babylonians and Indians, but it was the Greeks who first provided a proof, to which its discovery was often attributed to the Pythagorean school.

<b>Theorem 1. (Pythagoras' Theorem)</b> <i>In a right triangle, the square of the length of the hypotenuse is equal to the sum of the squares of the lengths of the other two sides.
$$
a^2 + b^2 = c^2
$$
where $c$ is the length of the hypotenuse and $a$ and $b$ are the lengths of the other two sides.</i>

<i>Proof.</i>

![pyth-thm](image/2025-06-25-real-number-04.jpg){: w="700"}

Let $\Delta ABC$ be right-angled triangle with $\angle ABC$ as the right angle. Produce $D$ on line $AC$ such that $BD$ is perpendicular to $AC$.

We would like to show that $\Delta ADB\sim \Delta ABC$ and $\Delta BDC\sim \Delta ABC$. 

First, $\Delta ADB$ and $\Delta ABC$ shares the same common angle $\angle BAC$. Moreover, since $\angle ABC$ and $\angle BDC$ are given to be right angle, by AA, $\Delta ADB\sim \Delta ABC$

Arguing similarly, $\Delta BDC$ and $\Delta ABC$ shares the same common angle $\angle ACB$. Also, $\angle ABC$ and $\angle BDC$ are right angles. By AA, $\Delta BDC\sim\Delta ABC$

By leveraging proportionality of the three sides, $\Delta ADB\sim \Delta ABC$ implies 

$$
\frac{AD}{AB} = \frac{AB}{AC}\\
AB^2 = AC\times AD
$$

Similarly, $\Delta BDC\sim\Delta ABC$ implies 

$$

\frac{BC}{AC} = \frac{DC}{BC}\\
BC^2 = AC\times DC
$$

Now since $\angle ADC$ equal two right angle, $A,D,C$ are collinear. Then we also have 
$$
AD + DC = AC
$$
Finally, we have 

$$
AB^2 + BC^2 = (AD+DC)\times AC = AC^2
$$
<br>&#x25A1;


The Pythagorean theorem prompted the discovery of incommesurable magnitudes (Or, in modern language, irrational numbers. But do be reminded that ancient Greeks did not view continuous magnitude as numbers). Consider a right triangle with both legs of length $1$ unit. By the Pythagorean theorem, the length of the hypotenuse is $\sqrt{2}$ unit. However, it can be proved that $\sqrt{2}$ is not a could never be represented as the ratio of two integers, which can be found in Euclid's <i>Elements</i>.

<b>Lemma 1. (Euclid's lemma)</b> <i>Let $p,m,n\in\mathbb{Z}$, where $p$ is a prime number. Suppose $p\mid mn$. Then $p|m$ or $p|n$.</i>

<i>Proof.</i> Omitted.<br>&#x25A1;

<b>Remark 1.</b> The original proof from the <i>Elements</i> is convoluted and difficult. While modern proofs of the lemma often involves Bezout's lemma, which states that for any integer $a,b$, if they are coprime ($\text{gcd}(a,b) =1$), then there is integer $s,t\in\mathbb{Z}$ such that $as + bt = 1$. To provide a rigorous proof from both ways would distract us to a lengthy detour. Interested reader can consult the <i>Elements</i> or any introductory textbook on number theory.

<b>Theorem 2.</b> <i>The number $\sqrt{2}$ is irrational.</i>

<i>Proof.</i> Suppose $\sqrt{2}$ is rational, then there is $m,n\in\mathbb{Z}$. where $\text{gcd}(m,n) = 1$, such that $\sqrt{2} = m/n$ , which means $m^2 = 2n^2$. Since $2\mid m^2$, Euclid's lemma implies that $2\mid m$. Then there is some $k\in\mathbb{Z}$ such that $m = 2k$. Substituting this equation to $m^2 = 2n^2$, we have $2k^2 = n^2$. Applying Euclid's lemma again, we have $2\mid n$. This contradicts the assumption that $\text{gcd}(m,n) = 1$. Therefore, $\sqrt{2}$ is irrational.<br>&#x25A1;

This fact shows that the rational numbers is <i>incomplete</i>, in the sense that not all quantity can be represented by a ratio of two integers. There are many "holes" in the rational line. 
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

## Real Numbers Form a Field
A field is a fancy way to say that we are able to perfrom addition, substraction, multicationa and division between elements in the sets. Where addition and multiplcation are equipped with the nice properties that we expect from usual algebraic operation, that is <i>commutativity</i>, <i>associativity</i>, and <i>distributivity</i>. 
Now, it is quite clear that we want to do all these operations on the real number line.

<b>Definition 1. (Field)</b> Let $\mathbb F$ be a set, and $+,\cdot:\mathbb F\times\mathbb F\to\mathbb F$ are binary operations such that the following are satisfied. 
1. <i>Commutativity.</i> For any $x,y\in \mathbb F$, $x+y=y+x$ and $x\cdot y = y\cdot x$.
2. <i>Associativity.</i> For any $x,y,z\in\mathbb F$, $x+(y+z) = (x+y) + z$ and $x\cdot(y\cdot z) = (x\cdot y) \cdot z$.
3. <i>Distributivity.</i> For any $x,y,z\in\mathbb F$, $x\cdot(y+z) = x\cdot y + x\cdot z$.
4. <i>Additive identity (Zero).</i> There exists a $0\in\mathbb F$ such that for any $x\in\mathbb F$, $x + 0 = 0$.
5. <i>Multiplicative identity (One).</i> There exists a $1\in\mathbb F$ such that for any $x\in\mathbb F$, $x \cdot 1 = x$.
6. <i>Additive inverse. </i> For any $x\in \mathbb F$, there exists a $-x\in\mathbb F$ such that $x + (-x) = 0$. 
7. <i>Multiplicative inverse.</i> For any non-zero $x\in\mathbb F$, there is a $x^{-1}\in\mathbb F$ such that $x \cdot x^{-1} = 1$.

Richard Dedekind was the first to formalise the idea of a field. According to Dedekind, this was his motivation:

> By a field we will mean every infinite system of real or complex numbers so closed in itself and perfect that addition, subtraction, multiplication, and division of any two of these numbers again yields a number of the system.

The key here is <i>closure</i>: Given any two numbers in the system, no matter what operation I do, the resultant element is going to be a number in the system. 

When we revisit the natural number, we would easily observe that it is not closed in subtraction. For example $1-2$ would give us something not in $\mathbb N$. The system of integer $\mathbb Z$ resolves the problem by adding negative numbers. However, $\mathbb Z$ is still not closed under division, which lead us to the formulation of rational numbers $\mathbb Q$. Now, to define the real numbers $\mathbb R$, we want this to also inherit this nice property of being closed. 

For the remainder of this section, I will prove some more properties that the real number system should possess. Or, to say it more generally, a field should possess. I know, they are going to be boring. But they are necessary.

<b>Proposition 1.</b> Let $\mathbb F$ be a field. Then its additive identity and multiplicative identity are unique. 

<i>Proof. </i> Let $0,0'\in\mathbb F$ both be additive identities. Then we have 
$$
\begin{align*}
0 &= 0 + 0' \tag{Additive identity}\\
&= 0' + 0 \tag{Commutativity}\\
&= 0' \tag{Additive identity}\\
\end{align*}
$$
Let $1,1'\in\mathbb F$ both be multiplicative identity. Then 
$$
\begin{align*}
1 &= 1 \cdot 1'  \tag{Multiplcative identity}\\
&= 1' \cdot 1 \tag{Commutativity}\\
&= 1' \tag{Multiplcative identity}\\
\end{align*} 
$$
<br>&#x25A1;

<b>Proposition 2.</b> Let $\mathbb F$ be a field. For any $x,y\in\mathbb F$, if $x + y = x$. Then $y= 0$.

<i>Proof.</i>
$$
\begin{align*}
y &= y + 0\tag{Additive identity}\\
&= y + (x - x)\tag{Addtive inverse}\\
&= (y+x) - x\tag{Associativity}\\
&= (x+y) - x\tag{Commutativity}\\
&= x - x\\
&= 0 \tag{Additive inverse}
\end{align*}
$$
<br>&#x25A1;

<b>Proposition 3</b> let $\mathbb F$ be a field. For any $x,y,z\in\mathbb F$, if $x + y = x + z$. Then $y = z$.
<i>Proof.</i>
$$
\begin{align*}
y &= y + 0 \tag{Additive identity}\\
&= y + (x-x)\tag{Additive inverse}\\
&= (y+x) - x\tag{Associativity}\\
&=(x+y) - x\tag{Commutativity}\\
&= (x+z) - x\\
&= (z+x) - x\tag{Commutativity}\\
&= z + (x-x)\tag{Associativity}\\
&= z + 0\tag{Additive inverse}\\
&= z\tag{Additive identity}
\end{align*}
$$
<br>&#x25A1;


<b>Proposition 4.</b> Let $\mathbb F$ be a field. Then for any $x\in\mathbb F$, $x\cdot 0 = 0$ 

<i>Proof.</i>
$$
\begin{align*}
x\cdot 0 &= x\cdot(0+0)\tag{Additive identity}\\
&= x\cdot 0 + x\cdot 0\tag{Distributivity}
\end{align*}
$$
By proposition 2, $x\cdot 0 = 0$.
<br>&#x25A1;


<b>Proposition 5.</b> Let $\mathbb F$ be a field. Then for any $x,y\in \mathbb F$, $(-x)\cdot y = x\cdot( -y) = -(x\cdot y)$

<i>Proof.</i>
$$
\begin{align*}
xy - xy &= 0\tag{Additive inverse}\\
&= y\cdot 0\tag{Proposition 3}\\
&= y\cdot(x - x)\tag{Additive inverse}\\
&= y\cdot x +y\cdot(-x)\tag{Distributivity}\\
&= x\cdot y + (-x)\cdot y\tag{Commutativity}
\end{align*}
$$
By proposition 3, we know $-xy = (-x)\cdot y$.
By a similar argument, we have
$$
\begin{align*}
xy - xy &= 0\tag{Additive inverse}\\
&= x\cdot 0\tag{Proposition 3}\\
&= x\cdot(y - y)\tag{Additive inverse}\\
&= x\cdot y +x\cdot(-y)\tag{Distributivity}\\
&= x\cdot y + x\cdot(-y)\tag{Commutativity}
\end{align*}
$$
By proposition 3, we have $-xy = x\cdot(- y)$.
<br>&#x25A1;

<b>Proposition 6.</b> Let $\mathbb F$ be a field. $\mathbb F$ is a singleton if and only if $1= 0$.

<i>Proof.</i>

($\Rightarrow$) This direction is obvious.

($\Leftarrow$) Suppose $1=0$. Then for any $x\in\mathbb F$, we have 
$$
\begin{align*}
x &= x\cdot 1\tag{Multiplicative identity}\\
&= x\cdot 0\\
&= x\cdot(1 - 1)\tag{Additive inverse}\\
&= x\cdot 1  + x\cdot(-1)\tag{Distributivity}\\
&= x\cdot 1 - x\cdot 1\tag{Proposition 5}\\
&= 0
\end{align*}
$$
Hence, $\mathbb F$ is a singleton. 
<br>&#x25A1;

Propositions I have proved here are nothing amazing. Even little kid uses them. I have reproduced their proof in great detail anyway, with the intent to emphasize that these proposition which we deem obvious are ultimately grounded by commutativity, associativity, and distributivity. 
## Real Numbers are Ordered

Take two distinct real numbers, we have mentioned that no matter how small the difference are, there are always a third number in between. Now to have a notion of betweeness, we necessarily presuppose orderedness in the real number line. For to say $c$ is between $a$ and $b$, is to say either $a < c < b$ or $b < c < a$. Moreover, it seemed betweenness only make sense if every two real number can be compared. 

Mathematician have found two ways to capture the idea of orderedness.

<b>Definition 2. (Order)</b> Let $X$ be a set and $R$ is a relation on $R$. $(X,R)$ is said to be an ordered set if it satisfies 

1. <i>Reflexivity.</i> For any $x\in X$, $xRx$.
2. <i>Anti-symmetry.</i> For any $x,y\in X$ if $xRy$ and $yRx$, then $x=y$.
3. <i>Transitivity.</i> For any $x,y,z\in X$, if $xRy$ and $yRz$, then $xRz$.

Moreover, $R$ is said be a total ordering if for any $x,y\in X$, either $xR y$ or $y Rx$.

<b>Definition 3. (Strict Order)</b> Let $X$ be a set and $R$ is a relation on $R$. $(X,R)$ is said to be an strict ordered set if it satisfies 

1. <i>Irreflexivity.</i> For any $x\in X$, $\lnot xRx$.
2. <i>Asymmetry.</i> For any $x,y\in X$ if $xRy$, then $\lnot yRx$. 
3. <i>Transitivity.</i> For any $x,y,z\in X$, if $xRy$ and $yRz$, then $xRz$.

Moreover, $R$ is said be a strict total ordering if for any $x,y\in X$, either $xR y$, $y Rx$, or $x=y$.

We usually denote ordering by $\leq$ or $\geq$, and strict ordering by $<$ or $>$. The notation implied the two definitions captures the idea of non-strict ordering that conveys the idea of "less than or equal to", and strict ordering conveys the idea of "less than and not equal to". Of course, this claim needs proof. 

<b>Proposition 7.</b> Let $(X, \leq)$ be an ordered set. Let $<$ be a relation defined by for any $x,y\in X$, $x < y$ if and only if $x\leq y$ and $x\neq y$. Then $<$ is a strict ordering. 

<i>Proof.</i>  
For irreflexivity, for any $x\in X$, since it is not true that $x\neq x$, then we have $\lnot x< x$. 

For asymmetry, suppose $x< y$, then $x\leq y$ and $x\neq y$. By anti-symmetry, we have $x\leq y\wedge y\leq x\to x=y$, which is equivalent to $x\leq y\to \lnot (y\leq x)\vee x=y$. Hence, we have either $\lnot(y\leq x)$ or $x=y$. But since we already have established $x\neq y$, we must have $\lnot(y\leq x)$. Then $\lnot(y\leq x) \vee x=y$ is also true, which means $\lnot(y\leq x \wedge x\neq y)$ is true. Hence, $\lnot y< x$. 

For transitivity, suppose $x< y$ and $y < z$, we have $x\leq y$, $y\leq z$, $x\neq y$ and $y\neq z$. By transitivity of $\leq$, we have $x\leq z$. It remains to show $x\neq z$. Suppose, on the contrary, that $ x = z$. Then we would have $x \leq y$ and $y\leq x$ simultaneously. By anti-symmetry, this means $x=y$, which is a contradiction. Therefore, we must have $x\neq z$.
<br>&#x25A1;

<b>Proposition 8.</b> Let $(X, <)$ be a strictly ordered set. Let $\leq$ be a relation defined by for any $x,y\in X$, $x \leq y$ if and only if $x< y$ or $x = y$. Then $\leq$ is a ordering. 

<i>Proof</i>

To show reflexivity, for any $x$, clearly $x=x$, so $x\leq x$.

To show anti-symmetry, suppose $x\leq y$ and $y\leq x$, we have $(x<y\vee x=y)$ and $(y< x\vee y=x)$. By De Morgan's law, we have $(x< y\wedge y<x)\vee x=y$. By asymmetry, $x<y\wedge y<x$ cannot be true, so we have $x=y$.

To show transitivity, if $x\leq y$ and $y \leq z$. We have four case. 
- <i>$x< y$ and $y< z$.</i> Transitivity implies $x < z$. Hence, $x\leq z$.
- <i>$x < y$ and $y = z$.</i> Immediately, $x < z$ and hence $x\leq z$
- <i>$x = y$ and $y< z$.</i> Immediately, $z < z$ and hence $x\leq z$
- <i>$x = y$ and $y = z$.</i> Clearly, $x=z$ and so $x\leq z$.

<br>&#x25A1;

Therefore, order and strict order are essentially the same thing. When we are talking about an ordered set, we can freely switch between "$\leq$" and $"<"$, depending on which one is more convenient for the situation.

How should the real numbers be ordered? Think back on the two iron rods. We already know that rod $A$ is longer than rod $B$. Symbolically, 

$$
\text{length}_A > \text{length}_B.
$$

Now imagine we were to <i>extend</i> the two rods by the same length, say 2 cm, the now extended rod $A$ should still be longer than extended rod $B$.

$$
\text{length}_A + 2cm > \text{length}_B + 2cm
$$

We could do the same thought experiment with <i>scaling</i> as well. Suppose we were to scale the length of the two rod by a factor of, say, 7. The scaled rod $A$ is still longer than the scaled rod $B$.

$$
5\times\text{length}_A > 5\times\text{length}_B
$$

I believe these two observation is obvious enough to everyone. Simple, but insightful, as these two formulation connected the notion of ordering with addition and multiplication. We have previously viewed the reals as a field and as an ordered set independently. Now, we can unify the two notion into one 

<b>Definition 4. (Ordered field)</b> Let $\mathbb F$ be a field and $<$ is an ordering on $\mathbb F$. $\mathbb F$ is a order field if it satisfy the following:
- for any $x,y,z\in\mathbb F$, $x< y$ implies $x+z < y+z$.
- for any $x,y,z\in\mathbb F$, where $z > 0$, $x < y$ implies $zx < zy$.

Now we know that the set of real numbers is a ordered field.

Okay. Here come some boring proposition proving. I will go over them more quickly this time. 

<b>Proposition 8.</b> Let $\mathbb F$ be an ordered field, then the following are true
1. For any non-zero $x\in\mathbb F$, $x > 0$ if and only if $-x < 0$.
2. For any non-zero $x\in\mathbb F$, $x^2 = x\cdot x >0$.
3. If $\mathbb F$ is not a singleton, $1>0$.
4. Every natural number is positive 

<i>Proof.</i> 

1).
$$
\begin{align*}
& x >0\\
\Leftrightarrow & x -x > -x\\
\Leftrightarrow & 0 > -x
\end{align*}
$$

2). Since $\mathbf F$ is strictly ordered, we have either $x< 0, x= 0$, or $x > 0$. Since $x$ is non-zero, we are left with $x>0 $ or $x<0$. If $x>0$, then the definition of ordered field grants that $x^2 >0$. If $x < 0$, then 1.) imples $-x >0$. Then we have 
$$
\begin{align*}
(-a)^2 - a^2 &= (-a)^2 + (-a)a\\
&= (-a)(-a+a)\\
&= 0\\
&= a^2 - a^2
\end{align*}
$$
Hence, $(-a)^2 = a^2$.

3.) Since $1\neq 0$, $1 = 1^2 > 0$.

4.) Let $P(n)$ be the proposition that $n > 0$. We have already proved the base case in 3.). It remains to prove the induction step. Suppose $k>0$ for some natural number $k$, then $k+1 > 1 > 0$. Transitivity grants that $k+1 > 0$.
<br>&#x25A1;

<b>Proposition 9.</b> Let $\mathbb F$ be an ordered field. Then the following hold:
1. If $x,y>0$, then $xy>0$.
2. $x > 0$ if and only if $x^{-1} > 0$
3. Suppose $x,y\in\mathbb F$ such that $xy>0$, then $x > 0$ and $y>0$, or $x< 0$ and $y < 0$. 
4. Suppose $x,y\in\mathbb F$ such that $xy < 0$, then $x < 0$ and $y>0$, or $x > 0$ and $y < 0$. 

<i>Proof.</i> 

1.) Since $x>0$, $y>0$, definition of ordered field grants $xy>0$.

2.) Suppose not, without loss of generality, then there is $x\in\mathbb F$ such that $x>0$ and $x^{-1} < 0$. Then we have $0 < x\cdot(-x^{-1}) = - (xx^{-1})= -1$. A contradiction.

3.)
$xy>0$ implies $x,y\neq 0$. Since if any one of them are zero, then $xy$ is zero.
Now suppose it is not the case that $x<0$ and $y<0$, then either $x>0$ or $y>0$. Without loss of generality, suppose $x>0$, then $x^{-1} > 0$ as well. Therefore,
$$
y = x^{-1}(xy) >0
$$

4.) Trivial logic exercise.
<br>&#x25A1;

## Real Numbers are Complete

Now on to the most important property of the real number--<i>Completeness</i>, i.e. there are no "gaps" on the real number line.

We can intuitively grasp, at least vaguely, what it means for something to have no gaps. But how do we formalise it? 
This is in fact a very challenging task. 
If a line is discontinuous, we cannot locate the gaps by directly pointing at them. Since gaps are exactly those points that are missing from the line. We need to locate these gaps indirectly. 

This was the problem that troubled Dedekind for a very long time. But finally, he came up with an ingenious idea. Imagine if we select a point from a straight line, then the remaining points will nicely sort themselves into two classes. Namely, those that are to the left of the selected point, and those that are to the right. Now Dedekind asks us to image the converse. He said 
> If all points of the straight line fall into two classes such that every point of the first class lies to the left of every point of the second class, then there exists one and only one point which produces this division of all points into two classes, this severing of the straight line into two portions.

So we have two classes $A_1$ and $A_2$. The two class have the property that for any $x\in A_1, y\in A_2$, $x_1 < x_2$. If our line is continuous, there is exactly a point $x^*$ that lies at the boundary of the two sets, i.e. $x_1 \leq x^* \leq x_2$.

Now this is a property a line with gaps lack. For exmaple, on the rational line, if we define 
$$
A_1 = \{x\in\mathbb{Q}\mid x<0 \text{ or }x^2 < 2\}\\
A_2 = \{x\in\mathbb{Q}\mid x>0 \text{ and }x^2 > 2\}
$$
Then $A_1$ and $A_2$ cuts $\mathbb{Q}$ into two parts

![rational-partition](image/2025-06-25-real-number-05.jpg){: w="700"}
_$A_1$ and $A_2$ cuts $\mathbb{Q}$ into two parts._

Note that we cannot find a point on $\mathbb Q$ that lies at the boundary of $A_1$ and $A_2$, since this point of division is exactly $\sqrt{2}$! But a continuous line can!

What all these characterisation amounts to is what modern mathematicians call the <i>least upper bound property</i>

<b>Definition 5. (Least upper bound/greatest lower bound)</b> Let $X$ be an ordered set and $A\subseteq X$ be a subset. $u\in X$ is an upper(lower) bound of $A$ if for any $x\in A$, $u \geq(\leq) x$.6

<b>Definition 6. (Least upper bound/greatest lower bound)</b> Let $X$ be an ordered set and $A\subseteq X$ be a subset. Suppose $u\in X$ is an upper(lower) bound of $A$. Then $u$ is the least upper bound (greatest lower bound) if for any upper bound (lower bound) $v\in X$, $u\leq(\geq) v$.

What a mouthful. Mathematician prefer to call a least upper bound the <i>supremum</i>, and the greatest lower bound the <i>infimum</i>. In our case, $\sqrt{2}$ is exactly the supremum of $A_1$, and the infimum of $A_2$. 

Now an important point to note is this: If we have a point, there is only one pair of cuts that have this specific point lying at their boundaries. What pair? Easy, given point $p$, the exact corresponding cuts are 

$$
B_1 = \{x:x<p\}\\
B_2 = \{x:x>p\}.
$$

But we should also notice that the converse is true. 

<b>Proposition 10.</b> Let $X$ be ordered and $A\subseteq X$ is bounded above. Then its supremum is unique.

<i>Proof.</i> Let $u,u'$ both be supremum of $A$. Since they are least upper bounds, $u\leq u'$ and $u'\leq u$. So $u=u'$.
<br>&#x25A1;

<b>Remark 2.</b> Mathematician uses $\sup A$ and $\inf A$ to denote $A$'s supremum and infimum.

Now there is a one-one correspondence between pairs of cuts and points.

$$
(A_1, A_2) \longleftrightarrow p
$$

Here's the cool thing. This point $p$ might or might not exist on the line; but the cut must necessarily exists. Since the cuts are defined in a way that refers to nothing but elements on the line (Recall that Dedekind define $A_1,A_2$ as a pair of sets such that for any $x_1\in A_2,x_2\in A_2$, $x_1<x_2$). Now we have a definition! We can look at the cuts of a line. If we find a particular cut whose supremum (of the left cut) and infimum (of the right cut) does not exists, then the line is discontinuous. Actually, if the supremum and infimum of cuts refers to the same point, why bother with a pair of sets when one is enough? Hence, we have our modern definition of continuity of a line. 

<b>Definition 7. (Dedekind completeness)</b> Let $X$ be an ordered set. $X$ is Dedekind complete if it satisfy the least upper bound property, that is, for any subseteq $A\subseteq X$ that is bounded above, $A$ has a supremum.

We have it. The real number system is a (Dedekind) complete ordered field!

## Properties of Complete Ordered Field and Aristotle's Concept of Continuity

TODO