<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#introduction'>Introduction</a>
  </li>
  <li>
    <a href='#possibility-trees-and-the-multiplication-rule'>Possibility Trees and the Multiplication Rule</a>
  </li>
  <li>
    <a href='#valid-and-invalid-arguments'>Valid and Invalid Arguments</a>
  </li>
  <li>
    <a href='#counting-elements-of-disjoint-sets'>Counting Elements of Disjoint Sets</a>
  </li>
</ol>
</details>

## Introduction
A <strong>sample space</strong> is the set of all possible outcomes of a random process or experiment. An <strong>event</strong> is a subset of a sample space

<div align="center">

<strong>Equally Likely Probability Formula</strong><br />

If $S$ is a finite sample space in which all outcomes are equally likely and $E$ is an event in $S$, then the <strong>probability of E</strong>, denoted <strong>P(E)</strong>, is

P( $E$ ) = the number of outcomes in $E$ / the total number of outcomes in $S$
</div> 

For any finite set $A$, $N(A)$ denotes the number of elements in $A$

<details>
    <summary>Example problem</summary>

An ordinary deck of cards contains 52 cards divided into four suits. The red suits are diamonds and hearts, and the black suits are clubs and spades. Each suit contains 13 cards of the following denominations: 2, 3, 4, 5, 6, 7, 8, 9, 10, J, Q, K, and A. The cards J, Q, and K are called face cards<br />

Consider the event that the chosen card is black and has an even number on it. Which of the following expresses this event as a set?
<ul>  
  <details>
    <summary>Solution</summary>

Set = {clubs: 2, 4, 6, 8, 10, spades: 2, 4, 6, 8, 10}<br />

The probability of this event is 10/52
</details>
</ul>  
</details>  

<details>
    <summary>Example problem</summary>

Two faces of a six-sided die are painted red, two are painted blue, and two are painted yellow. The die is rolled three times, and the colors that appear face up on the first, second, and third rolls are recorded

<ol type="a">
  <li>What is the probability of the event that exactly one of the colors that appears face up is red?</li>
  <li>What is the probability of the event that at least one of the colors that appears face up is red?</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>

Set = {RRR, RRB, RBR, RBB, BRR, BRB, BBR, RRY, RYR, RYY, YRR, YRY, YYR, YYY, YYB, YBB, YBY, BYY, BYB, BBY, BBB, YRB, YBR, BYR, BRY, RYB, RBY}

<ol type="a">
  <li>12/27</li>
  <li>19/27</li>
</ol>
</details>
</ul>  
</details>  

<details>
    <summary>Example problem</summary>

An urn contains two blue balls and three white balls. One ball is drawn from the urn, its color recorded, and is replaced. Another ball is then drawn and its color recorded

<ol type="a">
  <li>Consider the event that the first ball that is drawn is blue. Count all outcomes in this event. What is the total and what is the probability of the event?</li>
  <li>Consider the event that only the white balls are drawn. Count all the outcomes in this event. What is the total and what is the probability of the event?</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>

Set = {B1B2, B1B1, B2B1, B2B2, B1W1, B1W2, B1W3, B2W1, B2W2, B2W3, W1B1, W1B2, W2B1, W2B2, W3B1, W3B2, W1W1, W2W2, W3W3, W1W2, W1W3, W2W1, W2W3, W3W1, W3W2}

<ol type="a">
  <li>10</li>
  <li>10/25</li>
</ol>
</details>
</ul>  
</details>  

## Possibility Trees and the Multiplication Rule
A tree structure is useful tool for keeping systematic track of all possibilities in situations in which events happen in order

<details>
    <summary>Example problem</summary>

In a competition between players $X$ and $Y$, the first player to win three games in a row or a total of four games wins. How many ways can the competition be played if $X$ wins the first game and $Y$ wins the second and third games?
<ul>  
  <details>
    <summary>Solution</summary>

<img src="Images/Example Problems/Problem 1A.png" alt="Problem 1A">
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

A person buying a personal computer system is offered a choice of three models of the basic unit, four models of keyboard, the three models of printer. How many distinct systems can be purchased?
<ul>  
  <details>
    <summary>Solution</summary>

3 * 4 * 3 = 36 distinct models
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Suppose there are four routs from North Point to Boulder Creek, three routes from Boulder Creek to Beaver Dam, three routes from Beaver Dam to Star Lake, and two routes directly from Boulder Creek to Star Lake

<ol type="a">
  <li>How many routes from North Point to Star Lake pass through Beaver Dam?</li>
  <li>How many routes from North Point to Star Lake bypass Beaver Dam?</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>

<img src="Images/Example Problems/Problem 3A.png" alt="Problem 3A">
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Suppose that in a certain state, all automobile license plates have three uppercase letters followed by three digits

<ol type="a">
  <li>How many license plates are possible in which all the letters and digits are distinct?</li>
  <li>How many license plates could begin with AB and have all letters and digits distinct?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>26 * 25 * 24 * 10 * 9 * 8</li>
  <li>1 * 1 * 24 * 10 * 9 * 8</li>
</ol>
</details>
</ul>  
</details> 

### Permutations
A <strong>permutation</strong> of a set of objects is an ordering of the objects in a row

For any integer $n$ with $n \geq 1$, the number of permutations of a set with $n$ elements is $n!$

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>How many ways can the letters of the word DANCER be arranged in a row?</li>
  <li>How many ways can the letters of the word DANCER be arranged in a row if D and A must remain together, in order, as a unit?</li>
  <li>How many ways can the letters of the word DANCER be arranged in a row if the letters NCE must remain together, in order, as a unit?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>6 * 5 * 4 * 3 * 2 * 1 = 720</li>
  <li>4 * 3 * 2 * 1 = 24 * 5 = 120</li>
  <li>3 * 2 * 1 = 6 * 4 = 24</li>
</ol>
</details>
</ul>  
</details> 

### R-Permutation
An <strong>r-permutation</strong> of a set of $n$ elements is an ordered selection of $r$ elements taken from the set of $n$ elements

<div align="center">

$P$ $($ $n$ , $r$ $)$ $=$ $n$ $!$ $/$ $($ $n$ $-$ $r$ $)$ $!$ $)$
</div>

<details>
    <summary>Example problem</summary>

Evaluate the following quantities
<ol type="a">
  <li>
  
  $P(9, 5)$</li>
  <li>
  
  $P(9, 9)$</li>
  <li>
  
  $P(9, 4)$</li>
  <li>

  $P(9, 1)$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $P(9, 5)$ = 9! / (9 - 5)! = 9! / 4! = 9 * 8 * 7 * 6 * 5 = 15120</li>
  <li>
  
  $P(9, 9)$ = 9! / (9 - 9)! = 9! / 0! = 9! / 1 = 9! = 362880</li>
  <li>
  
  $P(9, 4)$ = 9! / (9 - 4)! = 9! / 5! = 9 * 8 * 7 * 6 = 3024</li>
  <li>

  $P(9, 1)$ = 9! / (9 - 1)! = 9! / 8! = 9</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>How many ways can the letters of the word DANCER be arranged in a row?</li>
  <li>How many ways can the letters of the word DANCER be arranged in a row if D and A must remain together, in order, as a unit?</li>
  <li>How many ways can the letters of the word DANCER be arranged in a row if the letters NCE must remain together, in order, as a unit?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>6 * 5 * 4 * 3 * 2 * 1 = 720</li>
  <li>4 * 3 * 2 * 1 = 24 * 5 = 120</li>
  <li>3 * 2 * 1 = 6 * 4 = 24</li>
</ol>
</details>
</ul>  
</details> 

### R-Permutation
An <strong>r-permutation</strong> of a set of $n$ elements is an ordered selection of $r$ elements taken from the set of $n$ elements

<div align="center">

$P$ $($ $n$ , $r$ $)$ $=$ $n$ $!$ $/$ $($ $n$ $-$ $r$ $)$ $!$
</div>

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>How many 4-permutations are there of a set of five objects?</li>
  <li>How many 2-permutations are there of a set of seven objects?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $P(5, 4)$ = 5! / (5 - 4)! = 5! / 1! = 5 * 4 * 3 * 2 = 120</li>
  <li>
  
  $P(7, 2)$ = 7! / (7 - 2)! = 7! / 5! = 7 * 6 = 42</li>
</ol>
</details>
</ul>  
</details> 

## Counting Elements of Disjoint Sets
### The Addition Rule
Suppose a finite set $A$ equals the union of $k$ distinct mutually disjoint subsets $A$<sub>1</sub>, $A$<sub>2</sub> ..., $A$<sub>k</sub>. Then

<div align="center">

$N$ $($ $A$ $)$ $=$ $N$ $($ $A$ <sub>1</sub> $)$ + $N$ $($ $A$ <sub>2</sub> $)$ + ... + $N$ $($ $A$ <sub>k</sub> $)$
</div>

<details>
    <summary>Example problem</summary>

Five-digit integers are integers from 10,000 from 99,999

<ol type="a">
  <li>How many five-digit integers are divisible by 5?</li>
  <li>What is the probability that a five-digit integer chosen at random is divisible by 5?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>First find the number of three-digit integers divisible by 5 and multiply that total by 10<br />
  100 - 199 that mod 5 = 0: 20 * 10 = 200<br />
  Then 200 by 10 since there are 10 thousands between 0 and 9,999 = 2000. Then multiply this by 9 since there are 9 ten-thousands between 10,000 and 99,999 = 18,000</li>
  <li>Probability = 18000 / (99999 - 10000) = 20%</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

In a certain country, license plates consist of zero or one digit followed by four or five uppercase letters from the Roman alphabet

<ol type="a">
  <li>How many different license plates can the country produce?</li>
  <li>How many license plates have no repeated letter?</li>
  <li>How many license plates have at least one repeated letter?</li>
  <li>WHat is the probability that a license plate has a repeated letter?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>If there are two options: no digit or one digit, then there are 11 options. These options include the 10 digits 0 - 9 and no digit at all<br />
  Since each license plate can have four or five uppercase letters, the total number of possibilities are: 11 * 26^4 + 11 * 26^5 = 5026736 + 130695136 = 135721872</li>
  <li>Total for four uppercase letters: 11 * 26 * 25 * 24 * 23 = 3946800<br />
  Total for five uppercase letters: 11 * 26 * 25 * 24 * 23 * 22 = 86829600<br />
  These two summed together is: 90776400</li>
  <li>Number of license plates that have at least one repeated letter = Total number of license plates - Total number of license plates that have no repeated letter = 135721872 - 90776400 = 44945472</li>
  <li>Probability = 44945472 / 135721872 = 33.1%
</ol>
</details>
</ul>  
</details> 

### The Difference Rule
If $A$ is a finite set and $B$ is a subset of $A$, then

<div align="center">

$N$ $($ $A$ $-$ $B$ $)$ $=$ $N$ $($ $A$ $)$ $-$ $N$ $($ $B$ $)$
</div>

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>How many strings of seven hexadecimal digits do not have any repeated digits?</li>
  <li>How many strings of seven hexadecimal digits have at least one repeated digit?</li>
  <li>What is the probability that a randomly chosen string of seven hexadecimal digits has at least one repeated digit?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $N$ = 16 * 15 * 14 * 13 * 12 * 11 * 10 = 57657600</li>
  <li>
  
  $N$ = Total number of elements = 16^7 - Total number of elements that do not have repeated digits = 16^7 - 5765700 = 210777856</li>
  <li>

  Probability = 210777856 / (210777856 + 57657600) = 210777856 / 268435456 = 78.5%</li>
</ol>
</details>
</ul>  
</details> 

### The Inclusion/Exclusion Rule
If $A$, $B$, and $C$ are any finite sets, then

<div align="center">

$N$ $($ $A$ $\vee$ $B$ $)$ $=$ $N$ $($ $A$ $)$ $+$ $N$ $($ $B$ $)$ $-$ $N$ $($ $A$ $\land$ $B$ $)$
</div>
