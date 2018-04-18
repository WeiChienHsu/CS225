# SET Theory


## Definitions and the Element Method of Proof

x is an element of S.

If S is a set and P(x) is a property that elements of S may or may not satisfy, then a set A may be defined by writing:

```
A = {x ∈ S | P(x)}
```

- The set of all x in S such taht P of x

***

## Subsets: Proof and Diproof

### set A to be a subset of a set B as formal universal conditional statement:

```
A ⊆ B <=> ∀x, if x ∈ A then x ∈ B
```

### The negation is:

```
A ⊊ B <=> ∀x, if x ∈ A then x ∉ B
```

### A proper subset of a set is a subset that is not equal to its containing set. Thus

```
A is a proper subset of B <=>
  1) A ⊆ B and,
  2) There is at least one element in B that not in A
```

## Basic Method for proving That one set is subset of another
Let sets X and Y be given. To prove that X ⊆ Y,
1. Suppose that x is a particular but arbitrarily chose element of Y.
2. Show that x is an element of Y.

### Proving and Disproving Subset Relations
Define sets A and B as fellows:

A = {m ∈ Z | m = 6r + 12 for some r ∈ Z }
B = {n ∈ Z | n = 3s for some s ∈ Z }

### Proof that A ⊆ B
Suppose x is a particular but arbitratily chosen element of A.
- [By definition of B, We must show that x = 3 * some integer. ]

By definition of A, there is an integer r such that x = 6r + 12
- [Does 6r + 12 = 3 * some integer?]

Let s = 2r + 4
- [We must check that s is an integer!]

Then s is an integer because products and sums of integers are integers.
- [Now we must check that x = 3s]

Also 3s = x
Thus, by definition of B, x is an element of B.


***

## Set Equality
Given sets A and B, A equals B, written A = B, if and only if every element fo A is in B and every element of B is in A.

```
A = B <=> A ⊆ B and B ⊆ A
```

Define sets A and B as fellows:

A = {m ∈ Z | m = 2a for some integer a }
B = {n ∈ Z | n = 2b - 2 for some integer b}

### Proofs
#### Proof That A ⊆ B
Suppore x is a particular but arbitrarily chosen element of A.
- [We must show gtaht x ∈ B, by definition of B, this means we need to show x = 2 * someinteger - 2]

By definition of A, there is an integer a such that x = 2a
- [Given that x = 2a, can x also be expressed as 2 * some integer - 2? b = (2a + 2)/2 = a + 1]
- [讓 x = 某個數 * 2 - 2，等於變成 2b - 2的格式]
- [x = I * 2 - 2]
- [直接讓 x = 2a = 2b - 2 || 得到 b = a + 1]
- [所以當 b = a + 1的時候，x可能為B的element，我們接著要證明 b 是 Integer]

Let b = a + 1
Then b is an integer because it is a sum of integers.
- [再把b放回n當中檢查，是否等於x]

Also 2b - 2 = 2(a+1) - 2 = 2a = x
Thus, by definition of B, x is an element of B.

***

## Operations on Sets
- The union of A and B: A ∪ B
- The intersection of A and B: A ∩ B
- The defference of B minus A(or relative complement of A in B): set of all elements that are in B and not A
- The complement of A, is the set of all elements in U that are not in A.

### Notation

- (a,b) = {x ∈ R | a < x < b}
- (a,b] = {x ∈ R | a < x <= b}
- (a,∞) = {x ∈ R | a > x }


### Unions and Intersections of an Indexed Collection of Sets
"The Union of the A-sub-i from i equals zero to n"

![sample](./image.png)


### Finding Unions and Intersections of More than Two Sets
For each postive integer i let Ai = { x ∈ R | -(1/i) < x < 1/i} = Ai = (-(1/i) * 1/i)

#### Find A1 U A2 U A3 and A1 ∩ A2 ∩ A3
1. Since all the elements in (-1/3, 1/3) and (-1/2, 1/2) are in (-1, 1): Ansewer is (-1, 1)
2. Answer is (-1/3, 1/3)

```
-|-----|------|----|---|-----|------|--
-1  -1/2    -1/3   0  1/3    1/2    1
```

##### Find U i = 1 to ∞ and ∩ i = 1 to ∞

1. = A1 U A2 U A3 U... A∞ = (-1, 1)

2. = A1 ∩ A2 ∩ A3 ∩... A∞ = (-1/ ∞, 1/ ∞) = {0}

***

## The Empty Set


***

## Power Set

∅ 
