# Logic Expressions: Part 1

## Propositions
A proposition is a declarative statement.

We often use letters p, q, r, s …. to denote propositions.
T: true F: false

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
- ⊕: exclusive or : Only one side could be false

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
| Laws| a | b |
|-----|---|---|
|Commutative| p ∧ q ⇐⇒ q ∧ p | p ∨ q ⇐⇒ q ∨ p |
|Associative| (p ∧ q) ∧ r ⇐⇒ p ∧ (q ∧ r) | (p ∨ q) ∨ r ⇐⇒ p ∨ (q ∨ r)|
|Distributive| p ∧ (q ∨ r) ⇐⇒ (p ∧ q) ∨ (p ∧ r)| p ∨ (q ∧ r) ⇐⇒ (p ∨ q) ∧ (p ∨ r)|
|Identity| p ∧ T ⇐⇒ p | p ∨ F ⇐⇒ p |
|Domination| p ∨ T ⇐⇒ T | p ∧ F ⇐⇒ F|
|Negation| p∨ ∼ p ⇐⇒ T | p∧ ∼ p ⇐⇒ F |
|Double Negative| ∼ (∼ p) ⇐⇒ p | |
|Idempotent| p ∧ p ⇐⇒ p  | p ∨ p ⇐⇒ p|
|De Morgan’s| ∼ (p ∧ q) ⇐⇒ (∼ p) ∨ (∼ q) | ∼ (p ∨ q) ⇐⇒ (∼ p) ∧ (∼ q)|
|Absorption| p ∨ (p ∧ q) ⇐⇒ p | p ∧ (p ∨ q) ⇐⇒ p|
|Conditional| (p =⇒ q) ⇐⇒ (∼ p ∨ q)  |∼ (p =⇒ q) ⇐⇒ (p∧ ∼ q)|

***

# Logic Expressions: Part 2