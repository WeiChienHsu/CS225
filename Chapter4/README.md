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

***

## 4.4
## Direct Proof and Counterexample : Quotient-Remainder Theorem (183 - 184)

***

## 4.6 
## Contradiction and Contraposition 



***

## 4.7
## Indirect Argument: Two Classiccal Theorems

***

## 4.8
## Application: Algorithms


***

## Require Reading

pp. 145- 159, 165-167, 170 - 174, 183-184, 201-203  ( Discrete Mathematics with Applications, Susanna S.Epp)
