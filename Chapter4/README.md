# Direct Proof & Contrapositive

- [4.1](#41)
- [4.2](#42)
- [4.3](#43)
- [4.4](#44)
- [4.6](#46)
- [4.7](#47)
- [4.8](#48)

***

## 4.1
## Direct Proof and Counterexample : Introduction

## Definitions - Odd and Even
An integer n is even if, and only if, n equals twice some integer. An integer n is odd if, and only if, n equals twice some integer plus 1.

- n is even <-> ∃ an integer k, such that n = 2k
- n is odd <-> ∃ and integer k, such that n = 2k + 1

```
If a and b are integer, is 6 a^2 * b even?
6 a^2 * b = 2 (3a^2*b) -> Since a and b are integer, then (3a^2*b) is integer too.
```

## Definitions - Prime
An integer n is prime if, and only if, n > 1 and for all positive integers r and s, if n = rs, then either r or s equals n.

An integer n is composite if, and only if, n > 1 and n = rs for some integers r and s with 1 < r < n and 1 < s < n.

## Proving Existential Statement
### Constructive proofs of existence

```
∃ x E D such that Q(x)

is ture if amd only if

Q(x) is true for at least one x in D
```

- One way to prove this is to find an x in D that make Q(x) true
- Another way is to give a set of directions for finding such an x.

### Disproving Universal Statements by Counterexample

To disprove a statement means to show that it si false. 

∀x in D, if P(x) -> Q(x)

Showing tha tthis statement false ie equivalent to showing that its negaiton is true:

∃x in D such that P(x) and ~Q(x)


### Proofs of Universal Statement
1. Copy the statement of the theorem to be proved on your paper.
2. Clearly mark the beginning of your proof with the word Proof.
3. Make your proof self-contained.
```
Since n is even, n = 2 s
```
4. Write your proof in complete, gramatically correct sentences.
```
Then m + n = 2r + 2s = 2(r+s)
```
5. Keep your reader informed about the status of each statement in your proof.
```
If something is assumed, preface it with a word like "Suppose or Assume".
```
6. Give a reason for each assertion in your proof.
```
by hoypothesis, by definitoin of 
```
7. Include the "little words and phrases" that make the logic of your arguments clear.
```
Let t = r + s. Then t is an integer because it s a sum of two integers
```
8. Display equations and in equalities.


### Direct Proof
1. Express the statement to be proved in the form "∀x E D, if P(x) then Q(x)"

2. Start the proof by supposing x is a particular but arbitarily chosen element of D for which the hypothesis P(x) is true. (Suppose x E D  and P(x))

3. Show that the conclusion Q(x) is true by using definitions, previouly established reults, and the rules for logicl inference.

***

## 4.2
## Direct Proof and Counterexample II : Rational Numbers(165 - 167)

A real number r is rational if and only if it can be expressed as a quotient of two integers with a nonzeri denominator. A real number that is not rational is irrational. More formally, if r is a real number, then

```
r is rational <=> ∃integers a and b such taht r = a / b and b != 0
```

### Is 0/2 a rational number or irrational number
rational number : No 2/0 is not a number (division by 0 is not allowed)
irrational number: No, every irrational number is a number.

### Is 0.12121212... a rational number
Yes. Let x = 0.121212... Then 100x = 12.12121212... Thus 
100x - x = 99x = 12 
x = 12 / 99

### Every Integer is a rational number
n = n / 1

### The Sum of any two rational numbers is rational
r + s = a / b  +  c / d  = ad + bc  / bd
Let p = ad + bc (sum or product of integers are integers)
Let q = bd 

r + s = p / q (q != 0) where p and q are integers 

thus r + s is rational

***

## 4.3
## Direct Proof and Counterexample III : Divisibility (170 - 174)
The notation d | n is read "d divides n" if n and d are integers and d != 0

d | n <=> ∃ an integer k such that n = dk

### A Positive Divisor of a Positive Integer
For all integers a and b, if a and b are positive and a divides b, then a <= b

### Divisors of 1
The only divisors of 1 are 1 and -1

### Divisibility by a Prime
#### Any integer n > 1 is divisible by a prime number.

Suppose n is a integer that is greater than 1. If n is prime, then n is divisible by a prime number.

If n is not prime:

```
n = r0 * s0 where r0 and s0 are integers and
  1 < r0 < n  and  1 < s0 < n
```
It follows by definition of divisibility that r0 | n.

If r0 is prime, then r0 is a prime number that divides n, and we're done.
But If r0 is not prime:

```
r0 = r1 * s1 where r1 and s1 are integers and
  1 < r1 < r0 and 1 < s1 < r0
```
It fellows by the definition of divisibility that r1 | r0.

We may continue in this way, factoring successive factors of n nutil we find a prime factor.

```
where k >= 0, 1 < rk < rk-1 < rk-2 < ... < r2 < r1 < r0 < n, and ri | n for each i = 0,1,2...,k-1,k.
The condition for termination is that rk should be prime. Hence rk is a prime number that divids n.
```

***

## 4.4
## Direct Proof and Counterexample : Quotient-Remainder Theorem (183 - 184)

### The Quotient-Reminder Theorem
Given any integer n and positive integer d, there exist unique integers q and r such that 
```
n = d*q + r and 0 < r < d
```

```
n div d = q
and
n mod d = r

<->

n = d * q + r
```
### The Parity of Consecutive Integers
Any two consecutive integers have opposite parity.

### Absolute Value and the Triangle Inequality
```
       x if x >= 0
|x| =  -x if x < 0
```
- For all real number r, -|r| <= r <= |r|
- For all real number r, |-r| = |r|
- For all real numbers x and y, |x + y| <= |x| + |y|
```
Case 1 

(x + y >= 0) : |x + y | = x + y 
and 
x <= |x| and y <= |y|
Hence,
|x+y| <= |x| + |y|

Case 2
(x + y < 0) : |x+y| = -(x+y) = -x + -y
and 
-x <= |-x| =|x| and -y <= |-y| < |y|
Hence,
|x+y| <= |x| + |y|
```

***
## Learning Objectives
- Understand and create proofs by contradiction
- Understand how to prove "If and only if" statement. (equvalences)
- Understand and create proofs by case
- Understand and create existence proofs(Constructive and Non-Constructive)

***

## 4.6 
## Contradiction and Contraposition (198-204)
What if the theorm statement is not naturally an implication?
"There is an inifinite number of prime number"
-> There is



## Contradiction
If you want to show that there is no object with a certain property, or if you want to show that a certain object does not have a certain property.

### Method of Proof by Contradiction 
1. Suppose the statement to be proved is fasle. That is, suppose that the negation of the statement is true.
2. Show that this suposition leads logically to a contradiction.
3. Conclude that the statement to be proved it true.


### There is no greatest integer.
1. Suppose there is a greatest integer N.
2. Then N >= n for every integern.
3. Let M = N + 1. Now M is an integer since it si a sum of integers.
4. Also M > N, So N is not a greatest Integer.

### There is no integer that is both even and odd
1. Suppose N is an integer, N = 2a for some integers a, which is a even.
2. N = 2b + 1 for some integers b.
3. 2a = 2b + 1, 2a - 2b = 1, a - b = 1/2
4. Scine a and b are integers, the difference between two integers need to be an integer as well.
5. Thus a - b is an integer, a - b is not an integer is a contradiction.


### The sum of any rational Number and any Irrational Number is Irrational
1. Suppose rational number + irrational number = rational number.
2. r + s is rational
```
a       c        ad - bc
- + s = -   s = ----------
b       d           bd

```
3. Now ab - bc is an integer, bd is an integer and != 0. 
4. Which means s is a rational number as well.
5. But we supposed s is a irrational, there is a contradiction.


## Proof of Equivalance (or Biconditional)

An integer n is postive if and only if -n is negative

P <-> Q, where P ≡ n > 0 and Q ≡ n < 0

To Prove that we need to Prove:

P -> Q
Q -> P

## Proof by case
Case1: n = 1
Case2: n = 2
Case3: n = -1.....


## Existence Proofs
There is a n > 0 that can be written as the sum of cubes of positive integers in two diff ways.

There exists an n such that P(n) :  ∃x P(x)

### Consrtuctive
Find a c in domain of discourse such that P(c) is true.


### Non-Constructive 
Prove existence WITHOUT explicitly identifying such a c

***


## Contrapostion
1. Express the statement to be proved in the form
- ∀x in D, if P(x) then Q(x)
2. Rewtire this statement in the contrapositive form 
- ∀x in D, if Q(x) is false then P(x) is false
3. Prove the contrapositive by a direct proof
- Suppose s is a (particular but arbitararily chosen) element of D such that Q(x) is false
- Show that P(x) is false

Note that when you use proof by contraposition, you know exactly what conclusion you need to show, namely the negaion of the hypothesis. Whereas in proof by contradiction, it may be difficult to know what contradiciton to head for.

Every statement that can be proved by contraposition can be proved by contradiction. But the converse is not true.


***

## For all integers n, if n^2 is even then n is even
### Contraposition
Suppose n is any odd integer.
By definition of odd, n = 2k + 1 for some integer k.
By substitution and algebra:
n^2 = (2K + 1) ^ 2 = 2(2k^2 + 2k) + 1
2k^2 + 2k is an integer since products and sums of integers are integers.
So n^2 is odd

### Contradiction 
Suppose not. Taht is, suppose there is an integer n such that n^2 is even and n is odd.
By the quotient-remainder theorem with d = 2, any integer is even or odd.
Hence, since it is odd and by definition of odd, n = 2k + 1 for some integer k.
n^2 = 2(2k^2 + 2k) + 1 which is also odd.
This contradicts Theorem 4.6.2 which states that no integer can be both even and odd.


***

## 4.7
## Indirect Argument: Two Classiccal Theorems(207-211)

### The √2 is irrational 
Suppose √2 is rational, then there are integers m and n with no common factors such that

√2 = m / n

Squaring both sides of equation gives

2 = m^2 / n^2
m^2 = 2n^2

Notes that m^2 is even.(2*X) If follows that m is even. We file this fact away for future reference and also deduce that:

m = 2k

Substituting equation1 in to equation2 we see that:

m^2 = 4k^2 = 2n^2

n^2 = 2k^2

Consequently, n^2 is even so do n is even. 
But we alos know that m is even. 
Hence both m and n have a common factor of 2. 
But this contradicts the supposition that m and n have non common factors.


### There are infinitely many prime numbers

Supoose the set of prime numbers is finite.
Then some prime number p is the largest of all the primes and henc we can list the prime numbers in ascending order:
2,3,5,7,...,p

Let N be the product of all the prime number + 1:
N = (2 * 3 * 5 * 7 * ... * p) + 1

Then, N > 1, N is divisible by some prime numebr q.

Because q is prime, q must equal one of the prime numbers in the set.
Thus, by definition of divisibllity, q divides 2*3*5*7..*p, but Not divide N

Hence "N is divisible by q" and "N is not dibisible by q" contradict!
We prove there are infinitely many prime numbers.

***

## 4.8
## Application: Algorithms


***

## Require Reading

pp. 145- 159, 165-167, 170 - 174, 183-184, 201-203  ( Discrete Mathematics with Applications, Susanna S.Epp)
