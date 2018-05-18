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
## Pigeonhole Principle

If ther are k containers and k+1 or more objects are placed in the containers, then at least one container has at least 2 objects.


### Example

Show that among any set of 5 positive integers, there are 2 with the same remainder when diveded by 4.

So, containers are {0, 1, 2, 3} which will be the possible remainders when diveded by 4.
And there are 5 positive integers. Thus, at least one conatiner(remainder) will hace two Objects(Integers)

-> At least one remainder will be used twice.

## Generalized Pigeonhole Principle

If N or more objects are placed in k containers, then at least one container must have at least [N/k] objects.

### Example

#### Consider a party with 100 people. What can we say about the number of people that were born in the same month?

Containers = 12 months
Object = 100 people
[100/12] = [8.3] = 9
At least one month has 9 people


#### Show that among any set of 9 positive integers, there are 3 with the same remainder when divided by 4.

Container = 4
Object = 9
[9/4] = [2.25] = 3

At least 3 number have the same remainder.


***



## Required Reading : pp. 525- 529, 540-549 