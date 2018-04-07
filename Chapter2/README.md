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

## Equivalency Truth Table

|P|~P|Q|~Q|R|(Q->R)|(P -> (Q->R)|(~Q vR)|~P v(~QvR)|
|-|--|-|--|-|:----:|:----------:|:-----:|:--------:|
|T|F |T|F |T|T     |T           |T      |T         |
|T|F |T|F |F|     |           |F      |F         |
|T|F |F|T |T|     |           |T      |T         |
|T|F |F|T |F|     |           |T      |T         |
|F|T |T|F |T|     |           |T      |T         |
|F|T |T|F |F|     |           |F      |T         |
|F|T |F|T |T|     |           |T      |T         |
|F|T |F|T |F|     |           |T      |T         |





