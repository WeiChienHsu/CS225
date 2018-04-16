# Direct Proof & Contrapositive

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

## Require Reading

pp. 145- 159, 165-167, 170 - 174, 183-184, 201-203  ( Discrete Mathematics with Applications, Susanna S.Epp)
