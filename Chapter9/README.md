# Basic Counting Rules

## Counting Problem
Specifies a set of objects with certain properties and asks how many such objects there are.

Break problem down into simpler problems via counting rules:
- Product Rule
- Sum Rule

### Product Rule
Suppose that each element to be counted can be described by a sequence of k choices, where the jth choice is the selection of an element from finite set Aj.

The totla number of elements is |A1| * |A2| * |Ak|

#### Example
Desinger can choose from:
- 5 diff styles = {style1, style2, style3...}
- 6 diff color = {color1, color2, color3...}
- 3 diff luxury = {luxury1, luxury2...}
Count the number of posibile designs:

5 * 3 * 6


### Sum Rule
Suppose that the set of elements to be counted can be expressed as the union of k disjoint sets A1, A2, ... Ak

The total number of elements is |A1| + |A2| + ... + |Ak|

A1 = {flight1, ...}
A2 = {bus1, ...}

There are 12 plane options, 5 bus options and 3 train options.

Totoal options is 12 + 5 + 3 = 20


## Combining Sum & Product Rules

A password must contain from 6 to 8 case-senstive alpha-numeric characters.

How many possible passwords are there?

Let P be the set of all passwords.

P = P6 U P7 U P8

#### Sume Rule # of passward = |P6| + |P7| + |P8|

Pn is a sequence of n choices of characters

Each choice has 26 + 26 + 10 = 62 elements

#### Product Rule: |Pn| = 62^n

#### #Of all passwords are 62^6 + 62^7 + 62^8

***

# Break the problem
Passwords must contain exactly 5 case-senstive alpha-numeric
characters and mush have at least one digit.

P5 = set of 5 character passwords(possibly without digits)
A5 = set of 5 character passwords without any digits

Passwords = |P5| - |A5| = 62^5 - 52^5


# Subset Exclusion
Suppose the set of element to be counted is the difference of two sets A-B, where B C A.

The total number of element is |A| - |B|


# Inclusion Exclusion Principle
Suppose that the set of elements to be counted can be expressed as the union of two possibly non-disjoint sets A and B

The total number of elements is |A| + |B| - |A^B|


***



## Required Reading : pp. 525- 529, 540-549 