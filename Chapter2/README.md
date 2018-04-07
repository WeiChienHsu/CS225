# Logic Expressions

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


## Equivalency Truth Table

|P|~P|Q|~Q|R|(Q->R)|(P -> (Q->R)|(~Q vR)|~P v(~QvR)|
|-|--|-|--|-|:----:|:----------:|:-----:|:--------:|
|T|F |T|F |T|T     |T           |T      |T         |
|T|F |T|F |F|F     |F           |F      |F         |
|T|F |F|T |T|T     |T           |T      |T         |
|T|F |F|T |F|T     |T           |T      |T         |
|F|T |T|F |T|T     |T           |T      |T         |
|F|T |T|F |F|F     |T           |F      |T         |
|F|T |F|T |T|T     |T           |T      |T         |
|F|T |F|T |F|T     |T           |T      |T         |


## Logic Symbols
≥ ≤ ≠ ¬ ∧ ∨ ⊕ ≡ → ↔ ∃ ∀ ( You can use either ~ or ¬ as negation symbol )

## Set Symbols
∈ ∉ ⊆ ⊂ ⊇ ⊃ ∅ ∪ ∩ ×


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
|Conditional (p =⇒ q) ⇐⇒ (∼ p ∨ q)  |∼ (p =⇒ q) ⇐⇒ (p∧ ∼ q)|
