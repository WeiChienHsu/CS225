# Logic Expressions: Part 1

## Propositions
A proposition is a declarative statement.

We often use letters p, q, r, s …. to denote propositions.
T: true F: false

A statement(proposition) is a sentence that is true or false but not both.

## Negation Operator
The truth value of ¬p is the opposite of p.

- Let p be “Tom is a human”
- If p is True then ¬p is “Tom is not a human.”

## Conjunction Operator
The conjunction of p and q is p ∧ q.

- p ∧ q is true if and only if p and q are both true

## Disjunction Operator
The disjunction of p and q is p ∨ q. 

- p ∨ q is true if and only if p is true or q is true

## Exclusive Or
- ⊕: exclusive or : Only one side could be false
- (p v q) ∧ ~(p ∧ q) : When or is used in its exclusve sense, the statement "p or q" means "p or q but not both" or " p or q and not both p and q".

## Implication Operator
The proposition (or statement) p → q has a truth value for
any setting of p and q.

- “If tomorrow is sunny then John will go jogging.”
-     |----p-----------|     |---q---------------|
- We don't know what John will do tomorrow if it isn't a sunny day
- The proposition “p implies q” is written p → q.
- Meaning: “If p is true then q must be true”
- “If p is false then q could be either true or false”

|P|Q|P -> Q|
|-|-|------|
|T|T|T|
|T|F|F|
|F|T|T|
|F|F|T|

## Biconditional
The truth table for A <-> B also written as A ≡ B, A = B

|P|Q|R|P ≡ Q|-R|-R ⊕ Q |(P ≡ Q) v (-R ⊕ Q )|  
|-|-|-|-----|--|:-----:|:-----------------:|
|T|T|T|T    |F |T      |T           |
|T|T|F|T    |T |F      |T           |
|T|F|T|F    |F |F      |F           |
|T|F|F|F    |T |T      |T           |
|F|T|T|F    |F |T      |T           |
|F|T|F|F    |T |F      |F           |
|F|F|T|T    |F |F      |T           |
|F|F|F|T    |T |T      |T           |

## Equivalency Truth Table

|P|~P|Q|~Q|R|(Q->R)|(P -> (Q->R)|(~Q vR)|~P v(~QvR)|P ≡ Q|P ⊕ Q| P ∨ Q | P ∧ Q |  
|-|--|-|--|-|:----:|:----------:|:-----:|:--------:|:---:|:---:|:-----:|:-----:|
|T|F |T|F |T|T     |T           |T      |T         |T    |F    |T      |T      |
|T|F |T|F |F|F     |F           |F      |F         |T    |F    |T      |T      |
|T|F |F|T |T|T     |T           |T      |T         |F    |T    |T      |F      |
|T|F |F|T |F|T     |T           |T      |T         |F    |T    |T      |F      |
|F|T |T|F |T|T     |T           |T      |T         |F    |T    |T      |F      |
|F|T |T|F |F|F     |T           |F      |T         |F    |T    |T      |F      |
|F|T |F|T |T|T     |T           |T      |T         |T    |F    |F      |F      |
|F|T |F|T |F|T     |T           |T      |T         |T    |F    |F      |F      |


## Logic Symbols
≥ ≤ ≠ ¬ ∧ ∨ ⊕ ≡ → ↔ ∃ ∀ ( You can use either ~ or ¬ as negation symbol )

## Set Symbols
∈ ∉ ⊆ ⊂ ⊇ ⊃ ∅ ∪ ∩ ×

## Logic Expression Example
1. If the patient is an infant then the patient has no children

- p: patient is an infant
- q: patient has child
- p -> -q

2. The file is either read-only or it is not read-only but is a copy.
- p: file read only
- -p: file not read only
- q: file is copy
- p v (-p ∧ q)

3. Bob is either rich or humble, but Bob is not humble if he is rich.
- but tranfer as and
- p: Bob is humble
- q: Bob is rich
- (p v q) ∧ (q -> -p)

## Logic Expression Example 2 (to English)
```
p: Today is Monday
q: It is raining
r: It is hot
```
1. -p -> (q v r)
- If today is not Monday, then it is raning or hot.

2. -(p v q) <-> r
- <-> if and only if
- It is not the case that it is Monday or it is raining, if and only if it is hot.

## Required Reading 
Chapter 2 ( Discrete Mathematics with Applications (4th Edition), Susanna S. Epp) Page : 23-36 ( You must try all the example problems from the book) 

***

# Table of Logical Equivalences
| Laws| a | b | Time to Use|
|-----|---|---|------------|
|Commutative| p ∧ q ≡ q ∧ p | p ∨ q ≡ q ∨ p | 變pq順序 |
|Associative| (p ∧ q) ∧ r ≡ p ∧ (q ∧ r) | (p ∨ q) ∨ r ≡ p ∨ (q ∨ r)|移動pqr相對位置|
|Distributive| p ∧ (q ∨ r) ≡ (p ∧ q) ∨ (p ∧ r)| p ∨ (q ∧ r) ≡ (p ∨ q) ∧ (p ∨ r)| 簡化邏輯式，或展開邏輯|
|Identity| p ∧ T ≡ p | p ∨ F ≡ p | and T / or F 不改變自身TF |
|Domination| p ∨ T ≡ T | p ∧ F ≡ F| or T / and F 改變自身為 T F |
|Negation| p∨ ∼ p ≡ T | p∧ ∼ p ≡ F | q 和 ~q -> 不可能 / q 與 ~q -> T |
|Double Negative| ∼ (∼ p) ≡ p | | 抵銷~ |
|Idempotent| p ∧ p ≡ p  | p ∨ p ≡ p| 重複 p and p / p or p|
|De Morgan’s| ∼ (p ∧ q) ≡ (∼ p) ∨ (∼ q) | ∼ (p ∨ q) ≡ (∼ p) ∧ (∼ q)|將~放入其中，改變and / or |
|Absorption| p ∨ (p ∧ q) ≡ p | p ∧ (p ∨ q) ≡ p| 簡化被覆蓋的部分 |
|Conditional| (p -> q) ≡ (∼ p ∨ q)  | ∼ (p -> q) ≡ (p ∧ ∼ q)| 條件轉換，前面~ 與後面 |

De Mogran : should change either V or ∧ to the opposite one.
- ~(P v ~Q)  ≡ ~P ∧ Q

Conditional: p -> q ≡ (~p v q) 
![conditional](images/conditional.png)

The red area describes all members for which the material conditional is true, and the white area describes all members for which it is false. The material conditional differs significantly from a natural language's "if...then..." statement. It is only false when both the antecedent {\displaystyle A} A is true and the consequent {\displaystyle B} B is false.

***

# Logic Expressions: Part 2

## Testing whether two statements forms P and Q are logically Equivalent
1. Construct a truth table with one column for the truth values of P and another column for the truth values of Q.
2. Check each combination of truth values of the statement variables to see whether the truth value of P is the same as the truth value of Q.

## De Morgan's Law
The negation of an "and" statement is logically equivalent to the "or" statement in which each component is negated.
The negation of an "or" statement is logically equivalent to the "and" statement in which each component is negated.

John is 6 feet tall and he weights at least 200 pounds.
- p: is 6 feet
- Q: is at least 200 pounds
- -> P ^ Q -> ~P V ~Q

John is not 6 feet tall or he weights less than 200 pounds

The bus was late or Tom's watch was slow
- The bus was not late and Tom's watch was not slow.

## Example
- Example 1:

```
Show that ∼(p ∨ ∼q) ∨ (∼p ∧ ∼q) ≡ ∼p.
L.H. S = ∼(p ∨ ∼q) ∨ (∼p ∧ ∼q) 1. De Morgan’s law
 ≡ (∼p ∧ ∼(∼q)) ∨ (∼p ∧ ∼q) 2. Double negation law
 ≡ (∼p ∧ q) ∨ (∼p ∧ ∼q) 3. Distributive law
 ≡ (∼p ∧ (q ∨∼q) ) 4. Negation law
 ≡ (∼p ∧ t ) 5. Identity law
 ≡ ∼p 
```

- Example 2:

```
Show that ∼ (q → p) ∨ (p ∧ q) ≡ q.
L.H.S = ∼ (q → p) ∨ (p ∧ q) 1. Implication / conditional equivalence
 ≡ ∼ (∼q ∨ p) ∨ (p ∧ q) 2. De Morgan’s law
 ≡ (∼ (∼q) ∧ ∼p) ∨ (p ∧ q) 3. Double negation law and commutative law (p ∧ q)
 ≡ (q ∧ ∼p) ∨ (q ∧ p) 4. Distributive law 
 ≡ (q ∧ (∼p ∨ p)) 5. Negation law
 ≡ (q ∧ T ) 6. Identity law
 ≡ q 
```

- Example 3:

```
Show that (p ∨ ∼q) ∧ (∼p ∨ ∼q) ≡∼q

(p ∨ ∼q) ∧ (∼p ∨ ∼q) 1. Commutative law
≡ (∼q ∨ p) ∧ (∼q ∨ ∼p) 2. Distributive law
≡ ∼q ∨ (p ∧ ∼p) 3. Negation law
≡ ∼q ∨ c 4. Identity law
≡ ∼q 
```
- Example 4:

```
L.H. S = (p ∧ q) → (p ∨ q) 1. Implication equivalence
≡ ∼ (p ∧ q) ∨ (p ∨ q) 2. De Morgan’s law
≡ (∼ p ∨ ∼ q) ∨ (p ∨ q) 3. Associative law
≡ (∼ p ∨ ∼ q ∨ p) ∨ q 4. Commutative law
≡ (∼ p ∨ p ∨ ∼ q) ∨ q 5. Associative law
≡ (∼ p ∨ p) ∨ (∼ q ∨ q) 6. Negation law
≡ t ∨ t 7. Idempotent law
≡ t, It’s a tautology
```

- Example 5:
```
L.H.S = (p∧q) → p 1.Implication equivalence
≡ ∼ (p∧q) ∨ p 2. De Morgan’s law
≡ ( ∼ p∨∼ q) ∨ p 3. Commutative law
≡ ( ∼ q∨∼p) ∨ p 4. Associative law
≡ ∼q∨ (∼p ∨ p) 5. Negation law
≡ ∼q∨ t 6. Universal bound law
≡ t , it’s a tautology.
```

- Example 6:
```
Show that ∼ ((∼p ∧ q) ∨ (∼p ∧ ∼q)) ∨ (p ∧ q) ≡ p.
L.H.S = ∼ ((∼p ∧ q) ∨ (∼p ∧ ∼q)) ∨ (p ∧ q) 1. De Morgan’s law
≡ (∼ (∼p ∧ q) ∧ ∼ (∼p ∧ ∼q)) ∨ (p ∧ q) 2. De Morgan’s law
≡ (∼(∼p) ∨ ∼ q) ∧ ((∼(∼p) ∨ ∼ (∼ q) ) ∨ (p ∧ q) 3. Double negation law
≡ ((p ∨ ∼ q) ∧ (p ∨ q)) ∨ (p ∧ q) 4. Distributive law
≡ ((p ∨ (∼ q ∧ q)) ∨ (p ∧ q) 5. Negation law
≡ (p ∨ c) ∨ (p ∧ q) 6. Identity law
≡ p ∨ (p ∧ q) 7. Absorption law
≡ p
```

- Example 7:
```
Show that (p → q) \/ (p → r) and p → (q \/ r) are logically equivalent.
L.H.S = (p → q) \/ (p → r) 1. Implication Equivalence
≡ (∼p \/ q) \/ (∼p \/ r) 2. Associative law
≡ ∼p \/ q \/ ∼p \/ r 3. Commutative law 
≡ ∼p \/∼p \/ q \/ r 4. Idempotent law
≡ ∼p \/ (q \/ r) 5. Implication law
 ≡ p → q \/ r , they are logically equivalent.
```

- Example 8:
```
Show that ∼ (p ∨ (¬p ∧ q)) ≡ (∼p ∧ ∼q) ∨ c.
L.H.S = ∼ (p ∨ (¬p ∧ q)) 1. De Morgan’s law
 ≡ ∼p ∧ ∼ (∼p ∧ q) 2. De Morgan’s law
 ≡ ∼p ∧ [∼ (∼p) ∨ ∼q] 3. Double negation law
 ≡ ∼p ∧ (p ∨ ∼q) 4. Distributive law
 ≡ (∼p ∧ p) ∨ (∼p ∧ ∼q) 5. Negation law
 ≡ c ∨ (∼p ∧ ∼q) 6. Commutative law
 ≡ (∼p ∧ ∼q) ∨ c 7. Identity law
 ≡ ∼p ∧ ∼q 
```

## Required Reading
Chapter 2 ( Discrete Mathematics with Applications (4th Edition), Susanna S. Epp) Page : 39-48 ( You must try all the example problems provided in the book) 