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
    <a href='#counting-elements-of-disjoint-sets'>Counting Elements of Disjoint Sets</a>
  </li>
  <li>
    <a href='#the-pigeonhole-principle'>The Pigeonhole Principle</a>
  </li>
  <li>
    <a href='#counting-subsets-of-a-set-combinations'>Counting Subsets of a Set: Combinations</a>
  </li>
  <li>
    <a href='#r-combinations-with-repetition-allowed'>r-Combinations with Repetition Allowed</a>
  </li>
  <li>
    <a href='#pascals-formula-and-the-binomial-theorem'>Pascal's Formula and the Binomial Theorem</a>
  </li>
  <li>
    <a href='#probability-axioms-and-expected-value'>Probability Axioms and Expected Value</a>
  </li>
  <li>
    <a href='#conditional-probability'>Conditional Probability</a>
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

A class of 233 students meets twice a week for lecture, after which they separate into eight breakout groups for discussion. What si the smallest number of students that can be in the largest breakout group? 
<ul>  
  <details>
    <summary>Solution</summary>

233 / 8 = 29.125. So we have seven groups of 29 and one group of 30. The answer is 30
</details>
</ul>  
</details>  

<details>
    <summary>Example problem</summary>

An urn contains 2 red balls and 2 blue balls. Balls are drawn randomly until all balls of one color have been removed and then we stop drawing. On average, how many balls will be remaining in the urn once we stop?
<ul>  
  <details>
    <summary>Solution</summary>

Outcomes: RR, BB, BRR, RBR, BRB, RBB<br />
Average number of balls pulled: 1/6 * (2 + 2 + 3 + 3 + 3 + 3) = 16/6 = 8/3<br />
Number of balls left: 12/3 - 8/3 = 1.67
</details>
</ul>  
</details>  

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

A coin is weighted so that heads comes up twice as often as tails. What is the expected number of heads in 72 tosses? 
<ul>  
  <details>
    <summary>Solution</summary>

72 * 2/3 = 48 heads
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

<details>
    <summary>Example problem</summary>

You have a fourteen eight-sided dice which are red and eleven six-sided dice which are blue. The dice are all far. You roll all the dice and then take the sum of the red dice an then subtract the sum of the blue dice. What is the expected average result? 
<ul>  
  <details>
    <summary>Solution</summary>

Expected value = $(1 + n) / 2$<br />
Expected value (red) = $(1 + 8) / 2 = 4.5$<br />
Expected value (blue) = $(1 + 6) / 2 = 3.5$<br />
Average = $14 * 4.5 - 11 * 3.5 = 24.5$
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

$P$ $($ $n$ , $r$ $)$ $=$ $n$ $!$ $/$ $($ $n$ $-$ $r$ $)$ $!$
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
  <li>Probability = 44945472 / 135721872 = 33.1%</li>
</ol>
</details>
</ul>  
</details> 


<details>
    <summary>Example problem</summary>

At a certain company, passwords must be from 4 to 6 symbols long and composed from the 26 uppercase letters of the Roman alphabet, the ten digits, and 14 symbols

<ol type="a">
  <li>How many passwords are possible if repetition of symbols is allowed?</li>
  <li>How many passwords contain no repeated symbols?</li>
  <li>How many passwords have at least one repeated symbol?</li>
  <li>What is the probability that a password chosen at random has at least one repeated symbol?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>For passwords with 4 symbols: 50<sup>4</sup><br />
  For passwords with 5 symbols: 50<sup>5</sup><br />
  For passwords with 6 symbols: 50<sup>6</sup><br />
  Using the addition rule: 50<sup>4</sup> + 50<sup>5</sup> + 50<sup>6</sup> = 6250000 + 312500000 + 15625000000 = 15943750000</li>
  <li>For passwords with 4 symbols: 50 * 49 * 48 * 47 = 5527200<br />
  For passwords with 5 symbols: 50 * 49 * 48 * 47 * 46 = 254251200<br />
  For passwords with 6 symbols: 50 * 49 * 48 * 47 * 46 * 45 = 11441304000<br />
  Using the addition rule: 5527200 + 254251200 + 11441304000 = 11701082400</li>
  <li>Total passwords with at least one repeated symbol = Total passwords - Total passwords with no repeated symbols<br />
  Total = 15943750000 - 11701082400 = 4242667600</li>
  <li>Probability = 4242667600 / 15943750000 = 26.6%</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Nine new employees, two of whom are married to each other, are to be assigned nine desks that are lined up in a row. If the assignment of employees to desks is made randomly, what is the probability that the married couple will have adjacent desks?

<ol type="a">
  <li>What is the probability that the couple has adjacent desks?</li>
  <li>What is the probability that the couple has nonadjacent desks?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>Let's say these are the nine desks: ABCDEFGHI<br />
  Total ways to seat the nine people: 9! = 362880<br />
  Total ways to seat nine people with two people always sitting together: 8 * 7! = 40320. Now this is if one person always sits on the left and the other always sits on the right. Since we do not care about who sits on the left and who sits on the right, this number can be multiplied by 2<br />
  Probability = 80640 / 362880 = 22.2%</li>
  <li>Probability of nonadjacent desks = 1 - Probability of adjacent desks = 77.8%
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

$N$ $($ $A$ $\cup$ $B$ $)$ $=$ $N$ $($ $A$ $)$ $+$ $N$ $($ $B$ $)$ $-$ $N$ $($ $A$ $\cap$ $B$ $)$
</div>

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>How many integers from 1 through 1,000 are multiples of 5 or multiples of 7?</li>
  <li>Suppose an integer from 1 through 1,000 is chosen at random. What is the probability that the integer is a multiple of 5 or a multiple of 7?</li>
  <li>How many integers from 1 through 1,000 are neither multiples of 5 nor multiples of 7?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  To find the number of integers in 1,000 divided by 5, $N(A)$ = 200<br />
  To find the number of integers in 1,000 divided by 7, $N(B)$ = 142<br />
  LCM of 5 and 7 is 35 and dividing 1,000 by 35 = 28. This is done since there are multiples of 5 and 7 that are the same<br />
  $N(A \cup B) = N(A) + N(B) + N(A \cap B)$ = 200 + 142 - 28 = 314</li>
  <li>Probability = 314 / 1000 = 31.4%</li>
  <li>Number of integers from 1 through 1,000 are neither multiples of 5 nor multiples of 7 = 1000 - 314 = 686</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

A random number from 1 to and including 33,333 is chosen, where each number is as likely to be chosen as any other number. Determine the exact probability, a fraction, that the randomly chosen number is a multiple of 5, 7, or 11. The fact that there are $[b/d]$ integers from 1 to $b$ that are multiples of by $d$ will be helpful
<ol type="a">
  <li>
  
  $|M$ <sub>5</sub> $|$</li>
  <li>
  
  $ + |M$ <sub>7</sub> $|$</li>
  <li>
  
  $ + |M$ <sub>11</sub> $|$</li>
  <li>
  
  $ - |M$ <sub>5</sub> $ \land M$ <sub>7</sub> $|$</li>
  <li>
  
  $ - |M$ <sub>5</sub> $ \land M$ <sub>11</sub> $|$</li>
  <li>
  
  $ - |M$ <sub>7</sub> $ \land M$ <sub>11</sub> $|$</li>
  <li>
  
  $ + |M$ <sub>5</sub> $ \land M$ <sub>7</sub> $ \land M$ <sub>11</sub> $|$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $|M$ <sub>5</sub> $| = 33333 / 5 = 6666.6 = 6666$</li>
  <li>
  
  $ + |M$ <sub>7</sub> $| = 33333 / 7 = 4761.8 = 4761$</li>
  <li>
  
  $ + |M$ <sub>11</sub> $| = 33333 / 11 = 3030.3 = 3030$</li>
  <li>
  
  $ - |M$ <sub>5</sub> $ \land M$ <sub>7</sub> $| = |M$ <sub>35</sub> $| = 33333 / 35 = 952.4 = 952$</li>
  <li>
  
  $ - |M$ <sub>5</sub> $ \land M$ <sub>11</sub> $|= |M$ <sub>55</sub> $| = 33333 / 55 = 606.1 = 606$</li>
  <li>
  
  $ - |M$ <sub>7</sub> $ \land M$ <sub>11</sub> $= |M$ <sub>77</sub> $| = 33333 / 77 = 432.9 = 432$</li>
  <li>
  
  $ + |M$ <sub>5</sub> $ \land M$ <sub>7</sub> $ \land M$ <sub>11</sub> $| = |M$ <sub>385</sub> $| = 33333 / 385 = 86.5 = 86$</li>
  <li>

  $|M$ <sub>5</sub> $ \vee M$ <sub>7</sub> $ \vee M$ <sub>11</sub> $| = 6666 + 4761 + 3030 - 952 - 606 - 432 + 86 = 12553$</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>How many integers from 1 through 1,000 are multiples of 2 or multiples of 9?</li>
  <li>Suppose an integer from 1 through 1,000 is chosen at random. What is the probability that the integer is a multiple of 2 or a multiple of 9?</li>
  <li>How many integers from 1 through 1,000 are neither multiples of 2 nor multiples of 9?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  To find the number of integers in 1,000 divided by 2, $N(A)$ = 500<br />
  To find the number of integers in 1,000 divided by 9, $N(B)$ = 111<br />
  LCM of 2 and 9 is 18 and dividing 1,000 by 18 = 55. This is done since there are multiples of 2 and 9 that are the same<br />
  $N(A \cup B) = N(A) + N(B) + N(A \cap B)$ = 500 + 111 - 55 = 556</li>
  <li>Probability = 556 / 1000 = 55.6%</li>
  <li>Number of integers from 1 through 1,000 are neither multiples of 2 nor multiples of 9 = 1000 - 556 = 444</li>
</ol>
</details>
</ul>  
</details> 

## The Pigeonhole Principle
The <strong>Pigeonhole Principle</strong> states that a function from one finite set to a smaller finite set cannot be one-to-one: there must be at least two elements in the domain that have the same image in the co-domain

<details>
    <summary>Example problem</summary>

In a group of 700 people, must there be 2 who have matching first and last initials? Assume each person has a first and last name, and the initials are from the 26 letters of the roman alphabet. Let $A$ be the set of 700 distinct people and let $B$ be the set consisting of all possible combinations of first and last initials
<ul>  
  <details>
    <summary>Solution</summary>

The cardinality of $B$ is equal to 26 * 26 = 676. So, if a function is constructed from $A$ to $B$ that relates each of the 700 people to their initials, then by the pigeonhole rule, the function is not one-to-one. Therefore, in a group of 700 people, it is impossible that no two people have matching first and last initials. So the answer to the question is yes
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>Given any set of seven integers, must there be at least two that have the same remainder when divided by 6?</li>
  <li>Given any set of seven integers, must there be at least two that have the same remainder when divided by 8?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  To answer this question, let $A$ be the set of 7 distinct integers and let $B$ be the set of all possible remainders that can be obtained when an integer is divided by 6, which means that $B$ has 6 elements. Hence, if a function is constructed from $A$ to $B$ that relates each of the integers in $A$ to its remainder, then by the pigeonhole principle, the function is not one-to-one. Therefore, for the set of integers in $A$, it is impossible for all the integers to have different remainders when divided by 6. So, the answer to the question is yes</li>
  <li>The answer is no because the following set of seven integers satisfies this claim: {0, 1, 2, 3, 4, 5, 6}</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Let $T$ = {1, 2, 3, 4, 5, 6, 7, 8, 9}. If five integers are chosen from $T$, must there be two integers whose sum is 10?
<ul>  
  <details>
    <summary>Solution</summary>

No because if the following integers are chosen: 1, 2, 3, 4, and 5, no two of these integers summed together equals 10
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>If eight are chosen from between 1 and 12 inclusive, must at least one of them be odd?</li>
  <li>If ten integers are chosen from between 1 and 20 inclusive, must at least one of them be even?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>Yes because only 6 of the numbers from 1 to 12 are even</li>
  <li>No because the integers 1, 3, 5, 7, 9, 11, 13, 15, 17, and 19 could be chosen</li>
</ol>
</details>
</ul>  
</details> 

## Counting Subsets of a Set: Combinations
Let $n$ and $r$ be nonnegative integers with $r \leq n$. An <strong>r-combination</strong> of a set of $n$ elements is a subset of $r$ of the $n$ elements. The symbol

<div align="center">

$\binom{n}{r}$
</div>

which is read " $n$ choose $r$ ", denotes the number of subsets of size $r$ that can be chosen from a set of $n$ elements

The number of subsets of size $r$ that can be chosen from a set of $n$ elements, $\binom{n}{r}$, is given by the formula

<div align="center">

$\binom{n}{r}$ = $P$ $($ $n$ , $r$ $)$ $/$ $r$ $!$
</div>

or equivalently

<div align="center">

$\binom{n}{r}$ = $n$ $!$ $/$ $r$ $!$ $($ $n$ $-$ $r$ $)$ $!$
</div>

where $n$ and $r$ are nonnegative integers with $r \leq n$

The binomial coefficient $\binom{n}{r}$ is used for selecting distinct items from a set of distinct objects, where the order does not matter

<details>
    <summary>Example problem</summary>

Compute each of the following:

<ol type="a">
  <li>
  
  $\binom{6}{0}$</li>
  <li>
  
  $\binom{6}{1}$</li>
  <li>
  
  $\binom{6}{2}$</li>
  <li>
  
  $\binom{6}{3}$</li>
  <li>
  
  $\binom{6}{4}$</li>
  <li>
  
  $\binom{6}{5}$</li>
  <li>
  
  $\binom{6}{6}$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $\binom{6}{0} = 6! / (0!(6 - 0)!) = 6! / 1(6!) = 1$</li>
  <li>
  
  $\binom{6}{1} = 6! / (1!(6 - 1)!) = 6! / 1(5!) = 6$</li>
  <li>
  
  $\binom{6}{2} = 6! / (2!(6 - 2)!) = 6! / 2(4!) = 15$</li>
  <li>
  
  $\binom{6}{3} = 6! / (3!(6 - 3)!) = 6! / 3!(3!) = 20$</li>
  <li>
  
  $\binom{6}{4} = 6! / (4!(6 - 4)!) = 6! / 4!(2!) = 15$</li>
  <li>
  
  $\binom{6}{5} = 6! / (5!(6 - 5)!) = 6! / 5!(1!) = 6$</li>
  <li>
  
  $\binom{6}{6} = 6! / (6!(6 - 6)!) = 6! / 6!(0!) = 1$</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

A student council consists of 15 students

<ol type="a">
  <li>How many ways can a committee of eight be selected from the membership of the council?</li>
  <li>Two council members have the same major and are not permitted to serve together on a committee. How many ways can a committee of eight be selected from the membership of the council?</li>
  <li>Two council members insist on serving on committees together. If they cannot serve together, they will not serve at all. How many ways can a committee of eight be selected from the council membership?</li>
  <li>Suppose the council contains eight men and seven women. How many committees of six contain three men and three women? How many committees of six contain at least on woman?</li>
  <li>Suppose the council consists of three freshmen, four sophomores, three juniors, and five seniors. How man committees of eight contain two representatives from each class?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  </li>
  
  $\binom{15}{8} = 15! / (8!(15 - 8)!) = 15! / 8!(7!) = 1307674368000 / 203212800 = 6435$</li>
  <li>

  The number of ways to select a committee of eight that contains $A$ and not $B$ is: $\binom{13}{7} = 13! / (7!(13 - 7)!) = 13! / 7!(6!) = (13 * 12 * 11 * 10 * 9 * 8) / (6 * 5 * 4 * 3 * 2) = 1235520 / 720 = 1716$<br />

  The number of ways to select a committee of eight that contains $B$ and not $A$ is: $\binom{13}{7} = 13! / (7!(13 - 7)!) = 13! / 7!(6!) = (13 * 12 * 11 * 10 * 9 * 8) / (6 * 5 * 4 * 3 * 2) = 1235520 / 720 = 1716$<br />

  The number of ways to select a committee of eight that contains neither $A$ nor $B$ is: $\binom{13}{8} = 13! / (8!(13 - 8)!) = 13! / 8!(5!) = (13 * 12 * 11 * 10 * 9) / (5 * 4 * 3 * 2) = 154440 / 120 = 1287$<br />
  
  The total number of committees of eight that can be selected from the membership of the council is the sum of the number of committees with $A$ and not $B$, $B$ and not $A$, and neither $A$ nor $B$. Thus, the answer is 4719</li>
  <li>

  The number of ways to select a committee of eight that contains $A$ and $B$ is: $\binom{13}{6} = 13! / (6!(13 - 6)!) = 13! / 6!(7!) = (13 * 12 * 11 * 10 * 9 * 8) / (6 * 5 * 4 * 3 * 2) = 1235520 / 720 = 1716$<br />

  The number of ways to select a committee of eight that contains $A$ and $B$ is: $\binom{13}{8} = 13! / (8!(13 - 8)!) = 13! / 8!(5!) = (13 * 12 * 11 * 10 * 9) / (5 * 4 * 3 * 2) = 154440 / 120 = 1287$<br />

  The total number of committees of eight that can be selected from the membership of the council is the sum of the number of committees with $A$ and $B$ and neither $A$ nor $B$. Thus, the answer is 3003</li>
  <li>

  The number of ways to select a committees of six that contains three men and three women: $\binom{8}{3} * \binom{7}{3} = (8! / (3!(8 - 3)!)) * (7! / (3!(7 - 3)!)) = (8! / 3!(5!)) * (7! / 3!(4!)) = ((8 * 7 * 6) / (3 * 2)) * ((7 * 6 * 5) / (3 * 2)) = (336 / 6) * (210 / 6) = 56 * 35 = 1960$<br />

  The number of ways to select a committee of six that contains at least one woman = Number of total possible committees - Number of total possible committees with only men<br />
  Number of total possible committees: $\binom{15}{6} = (15! / 6!(15 - 6)!) * (15! / 6!(9!)) = ((15 * 14 * 13 * 12 * 11 * 10) / (6 * 5 * 4 * 3 * 2)) = 3603600 / 720 = 5005$<br />
  Number of total possible committees with no women: $\binom{8}{6} = (8! / 6!(8 - 6)!) * (8! / 6!(2!)) = ((8 * 7) / (2)) = 28$<br />
  Number of total possible committees with at least one woman: 5005 - 28 = 4977</li>
  <li>
  
  Total number of possible committees with at least two freshmen, two sophomores, two juniors, and five seniors: $\binom{3}{2} * \binom{4}{2} * \binom{3}{2} * \binom{5}{2} = (3! / 2!(3 - 2)!) * (4! / 2!(4 - 2)!) * (3! / 2!(3 - 2)!) * (5! / 2!(5 - 2)!) = 3 * 6 * 3 * 10 = 540$</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

An instructor gives an exam with fifteen questions. Students are allowed to choose any eleven to answer

<ol type="a">
  <li>How mandy different choices of eleven questions are there?</li>
  <li>Suppose six questions require proof and nine do not. How many groups of eleven questions contain four that require proof and seven that do not?How many groups of eleven questions contain at least one that requires proof?How many groups of eleven questions contain at most three that require proof?</li>
  <li>Suppose the exam instructions specify that at most one of questions 1 and 2 may be included among the eleven. How many different choices of eleven questions are there?</li>
  <li>Suppose the exam instructions specify that either both questions 1 and 2 are to be included among the eleven or neither is to be included. How many different choices of eleven questions are there?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $\binom{15}{11} = 15! / (11!(15 - 11)!) = 15! / 11!(4!) = (15 * 14 * 13 * 12) / (4 * 3 * 2) = 32760 / 24 = 1365$</li>
  <li>
  
  Total number of groups of eleven questions that contain four that require proof and seven that do not = Total number of groups of four questions that require a proof * Total number of groups of seven questions that do not require a proof:<br />
  Total number of groups of four questions that require a proof: $\binom{6}{4} = 6! / 4!(6 - 4)! = 6! / 2!(4!) = (6 * 5) / 2 = 15$<br />
  Total number of groups of seven questions that do not require a proof: $\binom{9}{7} = 9! / 7!(9 - 7)! = 9! / 7!(2!) = (9 * 8) / 2 = 36$<br />
  Total number of groups of eleven questions that contain four that require proof and seven that do not: 15 * 36 = 540<br />
  
  Total number of groups of eleven questions that contain at least one that requires proof = Total number of groups of eleven questions - Total number of groups of questions that do not require a proof<br />
  Total number of groups of questions that do not require a proof: $\binom{9}{11} = 0$<br />
  Total number of groups of eleven questions that contain at least one that requires proof = 1365 - 0 = 1365<br />
  
  Total number of groups of eleven questions that contain at most three that require a proof = Total number of groups of eleven questions with: 0 proofs and 11 non-proofs, 1 proof and 10 non-proofs, 2 proofs and 9 non-proofs, 3 proofs and 8 non-proofs<br />
  Total number of groups of eleven questions containing 0 proofs and 11 non-proofs: $\binom{6}{0} * \binom{9}{11} = 0$<br />
  Total number of groups of eleven questions containing 1 proofs and 10 non-proofs: $\binom{6}{1} * \binom{9}{10} = (6! / 1!(6 - 1)!) * 0 = 0$<br />
  Total number of groups of eleven questions containing 2 proofs and 9 non-proofs: $\binom{6}{2} * \binom{9}{9} = (6! / 2!(6 - 2)!) * (9! / 9!(9 - 9)!) = (6! / 2!(4!)) * (9! / 9!(0!)) = ((6 * 5) / 2) * 1 = 15$<br />
  Total number of groups of eleven questions containing 3 proofs and 8 non-proofs: $\binom{6}{3} * \binom{9}{8} = (6! / 3!(6 - 3)!) * (9! / 8!(9 - 8)!) = (6! / 3!(3!)) * (9! / 8!(1!)) = ((6 * 5 * 4) / (3 * 2)) * ((9) / 1) = 180$<br />
  Total number of groups of eleven questions that contain at most three that require a proof = 0 + 0 + 15 + 185 = 195</li>
  <li>

  Total number of groups of eleven questions that contain at most one of questions one and two = Total number of groups of eleven questions given that question one or two must be answered + Total number of groups of eleven questions given that neither question one nor two must be answered<br />
  Total number of groups of eleven questions given that question one or question two must be answered: $\binom{2}{1} * \binom{13}{10} = (2! / 1!(2 - 1)!) * (13! / 10!(13 - 10)!) = (2 / 1) * ((13 * 12 * 11) / (3 * 2)) = 2 * 286 = 572$<br />
  Total number of groups of eleven questions given that neither question one nor two must be answered: $\binom{13}{11} * \binom{13}{11} = 13! / 11!(13 - 11)! = (13 * 12) / (2) = 78$<br />
  Total number of groups of eleven questions that contain at most one of questions one and two = 572 + 78 = 650</li>
  <li>

  Total number of groups of eleven questions that either both questions 1 and 2 are to be included among the eleven or neither is to be included = Total number of groups of eleven questions that both questions 1 and 2 are included + Total number of groups of eleven questions that neither questions 1 nor 2 are included<br />
  Total number of groups of eleven questions that both questions 1 and 2 are included: $\binom{2}{2} * \binom{13}{9} = 1 * (13! / 9!(13 - 9)!) = (13 * 12 * 11 * 10) / (4 * 3 * 2) = 715$<br />
  Total number of groups of eleven questions that neither questions 1 nor 2 are included: $\binom{2}{0} * \binom{13}{11} = (2! / 0!(2 - 0)!) * (13! / 11!(13 - 11)!) = (13 * 12) / (2) = 78$<br />
  Total number of groups of eleven questions that either both questions 1 and 2 are to be included among the eleven or neither is to be included = 715 + 78 = 793</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Martian Poker is a game played where each player receives four cards from a deck of 119 cards, where there are 7 suits and 17 cards from each suit. The order in which the cards are received does not matter

<ol type="a">
  <li>How many possible four card Martian Poker hands are there?</li>
  <li>A flush in Martian Poker is any hand where all cards are the same suit. How many possible flushes are there in Martian Poker?</li>
  <li>What is the probability of being dealt a flush in Martian Poker, expressed as a percentage?</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $\binom{119}{4}$</li>
  <li>

  $\binom{17}{4} * 7$</li>
  <li>

  $(\binom{17}{4} * 7) / \binom{119}{4}$</li>
</ol>
</details>
</ul>  
</details>  

<details>
    <summary>Example problem</summary>

Two new drugs are to be tested using a group of 50 laboratory mice, each tagged with a number for identification purposes. Drug $A$ is to be given to 17 mice, drug $B$ is to be given to another 17 mice, and the remaining 16 mice are to be used as controls. How many ways can the assignment of treatments to mice be made?
<ul>  
  <details>
    <summary>Solution</summary>

Total number of groups of assignments in the study of drug $A$, drug $B$ and the control is = Total number of groups of assignments for drug $A$ * Total number of groups of assignments for drug $B$ * Total number of groups of assignments for the control group<br />
Total number of groups of assignments for drug $A$ = $\binom{50}{17} = 50! / 17!(50 - 17)! = 50! / 17!(33!)$<br />
Total number of groups of assignments for drug $B$ = $\binom{33}{17} = 33! / 17!(33 - 17)! = 33! / 17!(16!)$<br />
Total number of groups of assignments for control = $\binom{16}{16} = 1$<br />
Total number of groups of assignments in the study = $(50! / 17!(33!)) * (33! / 17!(16!))$
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>How many 17-bit strings contain exactly eight 1's?</li>
  <li>How many 17-bit strings contain at least fourteen 1's?</li>
  <li>How many 17-bit strings contain at least one 1?</li>
  <li>How many 17-bit strings contain at most one 1?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  Total number of groups of 17-bit strings that contain exactly eight 1's = $\binom{17}{8} = 17! / (8!(17 - 8)!) = 17! / (8!(9!)) = (17 * 16 * 15 * 14 * 13 * 12 * 11 * 10) / (8 * 7 * 6 * 5 * 4 * 3 * 2) = 980179200 / 40320 = 24310$</li>
  <li>

  Total number of groups of 17-bit strings that contain at least fourteen 1's = Total number of groups of 17-bit strings that contain exactly fourteen 1's + Total number of groups of 17-bit strings that contain exactly fifteen 1's + Total number of groups of 17-bit strings that contain exactly sixteen 1's + Total number of groups of 17-bit strings that contain exactly seventeen 1's<br />
  Total number of groups of 17-bit strings that contain at least fourteen 1's: $\binom{17}{14} + \binom{17}{15} + \binom{17}{16} + \binom{17}{17} = 834$</li>
  <li>Total number of groups of 17-bit strings that contain at least one 1 = 2<sup>17</sup> - 1 = 131071</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Suppose that five microchips in a production run of fifty are defective. A sample of seven is to be selected to be checked for defects

<ol type="a">
  <li>How many different samples of seven can be chosen from the production run of fifty?</li>
  <li>How many samples will contain at least one defective chip?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  Total different number of samples = $\binom{50}{7} = 99884400$</li>
  <li>

  Total number of samples that contain at least one defective chip = Total number of samples - Total number of samples that contain no defective chips<br />
  Total number of samples that contain no defective chips: $\binom{45}{7} = 45379620$<br />
  Total number of samples that contain at least one defective chip = 99884400 - 45379620 = 54504780</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Ten points labeled $A, B, C, D, E, F, G, H, I, J$ are arranged in a plane in such a way that no three lie on the same straight line

<ol type="a">
  <li>How many straight lines are determined by the ten points?</li>
  <li>
  
  How many of these straight lines do not pass through point $A$?</li>
  <li>How many triangles have three of the ten points as vertices?</li>
  <li>

  How many of these triangles do not have point $A$ as a vertex?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $\binom{10}{2} = 45$</li>
  <li>

  $\binom{9}{2} = 45$</li>
  <li>

  $\binom{10}{3} = 120$</li>
  <li>

  $\binom{9}{3} = 120$</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Five women (W) and five men (M) line up at a checkout counter. What is the exact probability, expressed as a fraction, that they are arranged from first to last as W, M, W, M, W, M, W, M, W, M?
<ul>  
  <details>
    <summary>Solution</summary>

$\binom{10}{5} = 252$<br />
Probability: 1/252
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

A fair coin is flipped ten times. What is the exact probability, expressed as a fraction, that the coin comes up tails exactly five times?
<ul>  
  <details>
    <summary>Solution</summary>

Probability of heads 5 times: (1/2) <sup>5</sup><br />
Probability of tails 5 times: (1/2) <sup>5</sup><br />
Probability: (1/2) <sup>5</sup> * (1/2) <sup>5</sup> = (1/2) <sup>10</sup><br />
Now, there are $\binom{10}{5}$ arrangements of 5 tails.<br />
Total probability: 252/1024
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Consider recording the letters in the word $TENNESSEE$

If the $N$'s are randomly placed first, how many ways are there to choose positions for them? If the $E$'s are randomly placed second, how many ways are there to choose positions for them? If the $S$'s are randomly placed third, how many ways are there to choose positions for them?If the $T$'s are randomly placed last, how many ways are there to choose positions for them? So, what is the total number of ways to reorder the letters in the word $TENNESSEE$?
<ul>  
  <details>
    <summary>Solution</summary>

$N$'s: $\binom{9}{2} = 36$<br />
$E$'s: $\binom{7}{4} = 35$<br />
$S$'s: $\binom{3}{2} = 3$<br />
$T$'s: $\binom{1}{1} = 1$<br />
$TENNESSEE$ = 36 * 35 * 3 * 1 = 3780
</details>
</ul>  
</details> 

## r-Combinations with Repetition Allowed
An <strong>r-combination with repetition allowed</strong>, chosen from a set $X$ of $n$ elements is an unordered selection of elements taken from $X$ with repetition allowed

The number of $r$-combinations with repetition allowed that can be selected from a set of $n$ elements is

<div align="center">

$\binom{r + n - 1}{r}$
</div>

This equals the number of ways $r$ objects can be selected from $n$ categories of objects with repetition allowed

<details>
    <summary>Example problem</summary>

A camera shop stacks eight different types of batteries, one of which is type A76. Assume there are at least 31 batteries of each type

<ol type="a">
  <li>How many ways can a total inventory of 31 batteries be distributed among the eight different types?</li>
  <li>How many ways can a total inventory of 31 batteries be distributed among the eight different types if the inventory must include at least four A76 batteries?</li>
  <li>How many ways can a total inventory of 31 batteries be distributed among the eight different types if the inventory includes at most three A76 batteries?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $\binom{31 + 8 - 1}{8 - 1} = \binom{38}{7} = 12620256$</li>
  <li>

  To start, allocate the required 4 A76 batteries. Since the inventory must include at least 4 A76 batteries, 31 - 4 = 27: $\binom{27 + 8 - 1}{8 - 1} = \binom{34}{7} = 5379616$</li>
  <li>

  If there are zero A76 batteries: $\binom{31 + 7 - 1}{7 - 1} = \binom{37}{6} = 2324784$<br />
  If there is exactly one A76 battery, the remaining 30 batteries must be distributed among the 7 other types of batteries, because we have already accounted for one of the eight battery types as A76: $\binom{30 + 7 - 1}{7 - 1} = \binom{36}{6} = 1947792$<br />
  If there are exactly two A76 batteries, $\binom{29 + 7 - 1}{7 - 1} = \binom{35}{6} = 1623160$<br />
  If there are exactly two A76 batteries, $\binom{28 + 7 - 1}{7 - 1} = \binom{34}{6} = 1344904$
  Total = 7240640</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

If $n$ is a positive integer, how many 5-tuples of integers from 1 through $n$ can be formed in which the elements of the 5-tuple are written in increasing order byt are not necessarily distinct? In other words, how many 5-tuples of integers ($h, i, j, k, m$) are there with $1 /leq h \leq i \leq j \leq k \leq m \leq n$?

<ul>  
  <details>
    <summary>Solution</summary>

$\binom{n + 5 - 1}{4} = \binom{n + 4}{5} = (n + 4)! / (5!(n - 1)!)$
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

How many solutions are there to the equation $a + b + c + d + e = 485$. If each of $a, b, c, d,$ and $e$ is an integer that is at least 10?

<ul>  
  <details>
    <summary>Solution</summary>

Let's say $A = a + 10, B = b + 10, C = c + 10, D = d + 10,$ and $E = e + 10$<br />
$a + b + c + d + e + 50 = 485$<br />
$a + b + c + d + e = 435$
$\binom{435 + 5 - 1}{5 - 1} = \binom{439}{4} = 1526494751$
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

How many solutions are there to the equation $a + b + c + d = 31$, if each variable is a non-negative integer?

<ul>  
  <details>
    <summary>Solution</summary>

$\binom{31 + 4 - 1}{4 - 1} = \binom{34}{3} = 5984$
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

How many solutions are there to the equation $a + b + c = 21$, if each variable is a positive integer?

<ul>  
  <details>
    <summary>Solution</summary>

To be a positive integer, each $a, b,$ and $c$ must be greater than or equal to one<br />
$A = a + 1, B = b + 1,$ and $C = c + 1$<br />
$A + B + C + 3 = 21$<br />
$A + B + C = 18$
$\binom{18 + 3 - 1}{3 - 1} = \binom{20}{2} = 190$
</details>
</ul>  
</details> 

<details>
<summary>Example problem</summary>

<ol type="a">
  <li>A store sells 8 colors of balloons with at least 29 of each color. How many different combinations of 29 balloons can be chosen?</li>
  <li>If the store has only 12 red balloons but at least 29 of each other color of balloon, how many different combinations of balloons can be chosen?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $\binom{29 + 8 - 1}{8 - 1} = \binom{36}{7} = 8347680$</li>
  <li>

  $\binom{29 + 7 - 1}{7 - 1} = \binom{35}{6} * \binom{12 + 1 - 1}{1 - 1} = 1623160$</li>
</ol>
</details>
</ul>  
</details> 

<details>
<summary>Example problem</summary>

How many integer solutions are there to $a + b + c + d + e \leq 38$ where each variable must be nonnegative?
<ul>  
  <details>
    <summary>Solution</summary>

$a + b + c + d + e + f = 38$<br />
$\binom{38 + 6 - 1}{6 - 1} = \binom{43}{5}$
</details>
</ul>  
</details> 

<details>
<summary>Example problem</summary>

How many integer solutions are there to $a + b + c + d + e = 38$ where each variable must be nonnegative, and at least one of the variables is odd?
<ul>  
  <details>
    <summary>Solution</summary>

A = 2a, B = 2b, C = 2c, D = 2d, E = 2e<br />
$A + B + C + D + E = 19$<br />
$\binom{19 + 5 - 1}{5 - 1} = \binom{23}{4}$
</details>
</ul>  
</details> 

## Pascal's Formula and the Binomial Theorem
### Pascal's Formula
Let $n$ and $r$ be positive integers and suppose $r \leq n$. Pascal's Formula states that
<div align="center">

$\binom{n + 1}{r}$ $=$ $\binom{n}{r - 1}$ $+$ $\binom{n}{r}$
</div>

### Binomial Theorem
Given any real numbers $a$ and $b$ any any nonnegative integer $n$, 

<div align="center">

$($ $a$ $+$ $b$ $)$ <sup>n</sup> $=$ <math>
  <munderover>
    <mo>&#x2211;</mo>  <!-- Σ symbol -->
    <mrow><mi>k</mi><mi>=</mi><mn>0</mn></mrow>  <!-- Bottom: i = 1 -->
    <mi>n</mi>                        <!-- Top: n -->
  </munderover>
</math>

$\binom{n}{k}$ $a$ <sup>n - k</sup> $b$ <sup>k</sup> $=$ $a$ <sup>n</sup> $+$ $\binom{n}{1}$ $a$ <sup>n - 1</sup> $b$ <sup>1</sup> + $\binom{n}{2}$ $a$ <sup>n - 2</sup> $b$ <sup>2</sup> $+$ ... $+$ <sup>1</sup> + $\binom{n}{n - 1}$ $a$ <sup>1</sup> $b$ <sup>n - 1</sup> $+$ $b$ <sup>n</sup>

</div>

<details>
    <summary>Example problem</summary>

Use the binomial theorem to expand the following expression

<div align="center">

$($ $u$ $-$ $v$ $)$ <sup>5</sup>
</div>

<ul>  
  <details>
    <summary>Solution</summary>

$u$ <sup>5</sup> $+$ $\binom{5}{1}$ $u$ <sup>5 - 1</sup> $(-v)$ <sup>1</sup> $+$ $\binom{5}{2}$ $u$ <sup>5 - 2</sup> $(-v)$ <sup>2</sup> $+$ $\binom{5}{3}$ $u$ <sup>5 - 3</sup> $(-v)$ <sup>3</sup> $+$ $\binom{5}{1}$ $u$ <sup>5 - 4</sup> $(-v)$ <sup>4</sup> + $(-v)$ <sup>5</sup> = $u$ <sup>5</sup> - 5 $u$ <sup>4</sup> $v$ + 10 $u$ <sup>3</sup> $v$ <sup>2</sup> - 10 $u$ <sup>2</sup> $v$ <sup>3</sup> + 5 $uv$ <sup>4</sup> - $v$ <sup>5</sup>    
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

What is the constant term in the expansion of $(2x + 3/x^2)$ <sup>9</sup> ?

<ul>  
  <details>
    <summary>Solution</summary>

$\binom{9}{3} * (2x)$ <sup>6</sup> $ * (3 / x^2)$ <sup>3</sup> = 145152
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

A coin is weighted so that on each coin flip, heads comes up with probability $p$ = 0.63. What is the probability that heads comes up exactly $k$ = 10 times on $n$ = 21 flips of the coin?

<ul>  
  <details>
    <summary>Solution</summary>

$\binom{21}{10} * (0.63)$ <sup>10</sup> $ * (0.37)$ <sup>11</sup>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Use the binomial theorem to expand the following expression

<div align="center">

$($ $u$ $-$ $3$ $v$ $)$ <sup>4</sup>
</div>

<ul>  
  <details>
    <summary>Solution</summary>

$u$ <sup>4</sup> $+$ $\binom{4}{1}$ $u$ <sup>4 - 1</sup> $(-3v)$ <sup>1</sup> $+$ $\binom{4}{2}$ $u$ <sup>4 - 2</sup> $(-3v)$ <sup>2</sup> $+$ $\binom{4}{3}$ $u$ <sup>4 - 3</sup> $(-3v)$ <sup>3</sup> + $(-3v)$ <sup>4</sup> = $u$ <sup>4</sup> - 12 $u$ <sup>3</sup> $v$ + 54 $u$ <sup>2</sup> $v$ <sup>2</sup> - 108 $u$ <sup></sup> $v$ <sup>3</sup> + 81 $v$ <sup>4</sup>    
</details>
</ul>  
</details> 

## Probability Axioms and Expected Value
### Probability Axioms
Let $S$ be a sample space. A <strong>probability function</strong> $P$ from the set of all events in $S$ to the set of real numbers satisfies the following three axioms: For all events $A$ and $B$ in $S$

<ol type="a">
  <li>

  $0 \leq P(A) \leq 1$</li>
  <li>

  $P( \empty )$ and $P(S) = 1$</li>
  <li>

  If $A$ and $B$ are disjoint, then the probability of the union of $A$ and $B$ is</li>
</ol>

<div align="center">

$P$ $($ $A$ $\cup$ $B$ $)$ $=$ $P$ $($ $A$ $)$ $+$ $P$ $($ $B$ $)$</div>

### Probability of the Complement of an Even
If $A$ is any event in a sample space $S$, then

<div align="center">

$P$ $($ $A$ <sup>c</sup> $)$ $=$ $1$ $-$ $P$ $($ $A$ $)$</div>

### Probability of a General Union of Two Events
If $S$ is any sample space and $A$ and $B$ are any events in $S$, then

<div align="center">

$P$ $($ $A$ $\cup$ $B$ $)$ $=$ $P$ $($ $A$ $)$ $+$ $P$ $($ $B$ $)$ $-$ $P$ $($ $A$ $\cap$ $B$ $)$</div>

<details>
    <summary>Example problem</summary>

Suppose $A$ and $B$ are events in a sample space $S$ and suppose that $P(A) = 0.7, P(B$ <sup>c</sup> $) = 0.1$, and $P(A \cap B) = 0.6$. What is $P(A \cup B)$?

<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $P(A \cup B) = P(A) + P(B) - P(A \cap B) = 0.4 + 0.5 - 0.3 = 0.6$</li>
  <li>

  $P(C) = S - 0.6 = 0.4$</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

You are considering the following lottery game: three balls are drawn at random from among 11 balls numbered 1 through 11. Players win the following prize amounts for guessing which balls are drawn:
<ul>
  <li>$220 for correctly guessing all three numbers</li>
  <li>$22 for correctly guessing exactly two of the three numbers</li>
  <li>$14 for correctly guessing exactly one of the three numbers</li>
</ul>

If the game costs $20, what is the expected (average) amount lost per play. Round the final answer to the nearest cent

<ul>  
  <details>
    <summary>Solution</summary>

Total possible combinations: $\binom{11}{3} = 11! / ((3!)(11 - 3)!) = 165$<br />
Number of ways to get all three numbers: $\binom{3}{3} * \binom{8}{0} = 1$<br />
Number of ways to get two numbers: $\binom{3}{2} * \binom{8}{1} = 3 * 8 = 24$<br />
Number of ways to get one number: $\binom{3}{1} * \binom{8}{2} = 3 * 28 = 84$<br />
Number of ways to get zero numbers: $\binom{3}{0} * \binom{8}{3} = 56$<br />
Average amount won: $(1 * (220 / 165)) * (24 * (22 / 165)) * (84 (14 / 165)) = 11.66$<br />
Average amount: $20 - 11.66 = 8.34$ lost per ticket sold
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Let $A$ and $B$ be events in a sample space $S$, and let $C = S - (A \cup B)$. Suppose $P(A) = 0.4, P(B) = 0.5,$ and $P(A \cap B) = 0.3$. Find each of the following: 

<ol type="a">
  <li>
  
  $P(A \cup B)$</li>
  <li>

  $P(C)$</li>
  <li>

  $P(A$ <sup>c</sup> $)$</li>
  <li>

  $P(A$ <sup>c</sup> $\cap$ $B$ <sup>c</sup> $)$</li>
  <li>

  $P(A$ <sup>c</sup> $\cup$ $B$ <sup>c</sup> $)$</li>
  <li>

  $P(B$ <sup>c</sup> $\cap C)$</li>
</ol>

<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $P(A \cup B) = P(A) + P(B) - P(A \cap B) = 0.4 + 0.5 - 0.3 = 0.6$</li>
  <li>

  $P(C) = S - 0.6 = 0.4$</li>
  <li>

  $P(A$ <sup>c</sup> $) = 1 - P(A) = 1 - 0.4 = 0.6$</li>
  <li>

  $P(A$ <sup>c</sup> $\cap$ $B$ <sup>c</sup> $) = P(A$ <sup>c</sup> $\cap$ $B$ <sup>c</sup> $)$ <sup>c</sup> = $1 - P(A \cup B) = 1 - 0.6 = 0.4$</li>
  <li>

  $P(A$ <sup>c</sup> $\cup$ $B$ <sup>c</sup> $) = P(A$ <sup>c</sup> $\cup$ $B$ <sup>c</sup> $)$ <sup>c</sup> = $1 - P(A \cap B) = 1 - 0.3 = 0.7$</li>
  <li>

  $P(B$ <sup>c</sup> $\cap C) = 0.4$</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Let $A$ and $B$ be events in a sample space $S$, and let $C = S - (A \cup B)$. Suppose $P(A) = 0.8, P(B) = 0.2,$ and $P(A \cap B) = 0.1$. Find each of the following: 

<ol type="a">
  <li>
  
  $P(A \cup B)$</li>
  <li>

  $P(C)$</li>
  <li>

  $P(A$ <sup>c</sup> $)$</li>
  <li>

  $P(A$ <sup>c</sup> $\cap$ $B$ <sup>c</sup> $)$</li>
  <li>

  $P(A$ <sup>c</sup> $\cup$ $B$ <sup>c</sup> $)$</li>
  <li>

  $P(B$ <sup>c</sup> $\cap C)$</li>
</ol>

<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $P(A \cup B) = P(A) + P(B) - P(A \cap B) = 0.8 + 0.2 - 0.1 = 0.9$</li>
  <li>

  $P(C) = S - 0.9 = 0.1$</li>
  <li>

  $P(A$ <sup>c</sup> $) = 1 - P(A) = 1 - 0.8 = 0.2$</li>
  <li>

  $P(A$ <sup>c</sup> $\cap$ $B$ <sup>c</sup> $) = P(A$ <sup>c</sup> $\cap$ $B$ <sup>c</sup> $)$ <sup>c</sup> = $1 - P(A \cup B) = 1 - 0.9 = 0.1$</li>
  <li>

  $P(A$ <sup>c</sup> $\cup$ $B$ <sup>c</sup> $) = P(A$ <sup>c</sup> $\cup$ $B$ <sup>c</sup> $)$ <sup>c</sup> = $1 - P(A \cap B) = 1 - 0.1 = 0.9$</li>
  <li>

  $P(B$ <sup>c</sup> $\cap C) = 0.1$</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

Let $A$ and $B$ be events in a sample space $S$, and let $C = S - (A \cup B)$. Suppose $P(A) = 0.4, P(B) = 0.5,$ and $P(A \cap B) = 0.3$. Find each of the following: 

<ol type="a">
  <li>
  
  $P(A \cup B)$</li>
  <li>

  $P(C)$</li>
  <li>

  $P(A$ <sup>c</sup> $)$</li>
  <li>

  $P(A$ <sup>c</sup> $\cap$ $B$ <sup>c</sup> $)$</li>
  <li>

  $P(A$ <sup>c</sup> $\cup$ $B$ <sup>c</sup> $)$</li>
  <li>

  $P(B$ <sup>c</sup> $\cap C)$</li>
</ol>

<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $P(A \cup B) = P(A) + P(B) - P(A \cap B) = 0.4 + 0.5 - 0.3 = 0.6$</li>
  <li>

  $P(C) = S - 0.6 = 0.4$</li>
  <li>

  $P(A$ <sup>c</sup> $) = 1 - P(A) = 1 - 0.4 = 0.6$</li>
  <li>

  $P(A$ <sup>c</sup> $\cap$ $B$ <sup>c</sup> $) = P(A$ <sup>c</sup> $\cap$ $B$ <sup>c</sup> $)$ <sup>c</sup> = $1 - P(A \cup B) = 1 - 0.6 = 0.4$</li>
  <li>

  $P(A$ <sup>c</sup> $\cup$ $B$ <sup>c</sup> $) = P(A$ <sup>c</sup> $\cup$ $B$ <sup>c</sup> $)$ <sup>c</sup> = $1 - P(A \cap B) = 1 - 0.3 = 0.7$</li>
  <li>

  $P(B$ <sup>c</sup> $\cap C) = 0.4$</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

A lottery game offers $3 million to the grand prize winner, $20 to each of 10,000 second prize winners, and $5 to each of 50,000 third prize winners. The cost of the lottery is $2 per ticket. Suppose that 2.5 million tickets are sold. What is the expected value of a ticket?

<ul>  
  <details>
    <summary>Solution</summary>

Total expected value of a ticket = $3000000 * (1 / 2500000) + 20 * (1/ 10000) + 5 * (1 / 50000) = 1.38$<br />
Total expected value of a ticket minus the cost of the ticket = $1.38 - 2 = -0.62$
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

A company offers a rattle whose grand prize is a $45,000 new car. Additional prizes are a $1,100 television and a $600 computer. Tickets cost $22 each. Ticket income over the cost of the prizes will be donated to charity. If 3,000 tickets are sold, what is the expected gain or loss of each ticket?

<ul>  
  <details>
    <summary>Solution</summary>

Total expected value of a ticket = $45000 * (1 / 3000) + 1100 * (1/ 3000) + 600 * (1 / 3000) = 1.38 = 15 + 0.37 + 0.2 = 15.57$<br />
Total expected value of a ticket minus the cost of the ticket = $15.57 - 22 = -6.43$
</details>
</ul>  
</details> 

## Conditional Probability
Let $A$ and $B$ be events in a sample space $S$. If $P(A) \neq 0$, then the <strong>conditional probability of B given A</strong>, denoted $P(B|A)$, is

<div align="center">

$P$ $($ $B$ $|$ $A$ $)$ $=$ $P$ $($ $A$ $\cap$ $B$ $)$ $/$ $P$ $($ $A$ $)$
</div>

### Independent Events
If $A$ and $B$ are events in a sample space $S$, then $A$ and $B$ are <strong>independent</strong> if, and only if,

<div align="center">

$P$ $($ $A$ $\cap$ $B$ $)$ $=$ $P$ $($ $A$ $)$ $*$ $P$ $($ $B$ $)$</div>

<details>
    <summary>Example problem</summary>

Let $A$ and $B$ be any events in some general sample space $S$. Write equivalent expressions  for which the equalities always hold

<ol>
  <li>

  $P(A \cap B)$</li>
  <li>

  $P(A \cup B)$</li>
  <li>

  $P(S)$</li>
</ol>

<ul>  
  <details>
    <summary>Solution</summary>

<ol>
  <li>

  $P(A \cap B) = P(A) + P(B) - P(A \cup B)$<br />
  $P(A \cap B) = P(B) * P(A | B)$<br />
  $P(A \cap B) = P(A) * P(B | A)$<br /></li>
  <li>

  $P(A \cup B) = P(A) + P(B) - P(A \cap B)$<br />
  </li>
  <li>

  $P(S) = P(A) + P(A$ <sup>c</sup> $)$<br />
  $P(S) = P(B) + P(B$ <sup>c</sup> $)$<br />
  $P(S) = 1$</li>
</ol>
</details>
</ul>  
</details> 

<details>
    <summary>Example problem</summary>

<ol>
  <li>

  Count the number of ways in which a coin can be flipped 10 times and land on heads exactly 5 times</li>
  <li>

  The number of 5-element subsets of a 10-element set</li>
  <li>

  The number of arrangements of ABABABABAB</li>
</ol>

<ul>  
  <details>
    <summary>Solution</summary>

<ol>
  <li>

  $\binom{10}{5} = 252$</li>
  <li>

  $\binom{10}{5} = 252$</li>
  <li>

  $\binom{10}{5} = 252$</li>
</ol>
</details>
</ul>  
</details> 
