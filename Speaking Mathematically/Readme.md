<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#variables'>Variables</a>
  </li>
  <li>
    <a href='#the-language-of-sets'>The Language of Sets</a>
  </li>
  <li>
    <a href='#the-language-of-relations-and-functions'>The Language of Relations and Functions</a>
  </li>
</ol>
</details>

## Variables
### Expressions, Variables, and Evaluation
An <strong>expression</strong> is a well-formed combination of symbols which possibly contain <strong>variables</strong>

An expression may be evaluated according to some rules, given an assignment of values to the variables

Functions can also be represented as a <strong>function</strong> such as $f(x) = x^2$

The <strong>set</strong> of all considered inputs to the function or variable(s) for which there is a valid evaluation according to the rules is called the <strong>domain</strong> of the function or variable(s)

A <strong>definition</strong> gives a statement of meaning to a term

A <strong>universal statement</strong> says that a certain property is true for all elements in a set. In other words, a property is true for every element in a set
<ul>
  <li>Every person in this class is a USF student</li>
</ul>

A <strong>conditional statement</strong> says that if one thing is true then some other thing also has to be true. In other words, the <strong>antecedent</strong> is true if the <strong>consequent</strong> is true
<ul>
  <li>If a person is in this class, they are a USF student</li>
</ul>

An <strong>existential statement</strong> says that there is at least one thing for which the property is true. In other words, a property is true for at least one element of a set
<ul>
  <li>Some person in this class is not a USF student</li>
</ul>

A <strong>universal conditional statement</strong> is a statement that is both universal and conditional
<ul>
  <li>For all people a, if a is a rich person, then a is a snob</li>
</ul>  

## The Language of Sets
A <strong>set</strong> is a well-defined collection of distinct objects known as <strong>members</strong> or <strong>elements</strong>

The notation $x \in A$, read as $x$ in $A$, indicates that the element $x$ is a member of the set $A$. The notation $x \notin A$ means that $x$ is not in $A$

The <strong>cardinality</strong> of a set $A$, denoted as $|A|$, is the number of elements contained in the set, where writing $|A| = \infty$ denotes that $A$ contains infinitely many elements

<ul>
  <li>$\mathbb{R}$ is the set of all <strong>real numbers</strong>. Real numbers are all the numbers that can be found on the number line</li>
  <li>$\mathbb{C}$ is the set of all <strong>complex numbers</strong>. Complex numbers consist of a real part and an imaginary part</li>
  <li>$\mathbb{Z}$ is the set of all <strong>integers</strong>. Integers are any positive or negative whole numbers</li>
  <li>$\mathbb{Q}$ is the set of all <strong>rational numbers</strong>. A rational number is any real number that is an integer or is a fraction</li>
  <li>$\mathbb{N}$ is the set of all <strong>natural numbers</strong>. A natural number is any integer greater than zero</li>
</ul>  

### Set-Roster Notation
A set may be specified using <strong>set-roster notation</strong> by writing all of its elements between braces. For example, the set $A$ = &#123; 1, 2, 3&#125; denotes the set whose elements are 1, 3, and 3

A variation of the notation is sometimes used to describe a very large set, as the set 
$A$ = &#123;1, 2, 3, ..., 100&#125; refers to the set of all integers from 1 to 100. The symbol ... is called an <strong>ellipsis</strong> and is read "and so forth"

Here is an example of using set-roster notation:

<div align="center">

$X$ = &#123;1, 2, 3&#125; $\quad Y$ = &#123;1, 3, 2&#125; $\quad Z$ = &#123;1, 2, 2, 3&#125;
</div>

Each of the above refers to the same three-element set, since listed order does not distinguish sets, and sets contain distinct objects, as sets allow elements to be listed repeatedly, but that is usually not a common practice

### Set-Builder Notation
Let $S$ denote a set and let $P(x)$ be a property that an element $x \in S$ may or may not have> Set $A$ can be introduced as in the following:

<div align="center">

$A$ = &#123; $x \in S | P(x)$ &#125;
</div>

### Subsets
If $A$ and $B$ are sets, then $A$ is called a <strong>subset</strong> of $B$, written $A \subseteq B$, if, and only if, every element of $A$ is also an element of $B$

Symbolically:

<div align="center">

$A \subseteq B \quad$ means that $\quad$ for all elements $x$, if $x \in A$ then $x \in B$ 
</div>

The phrases <em>$A$ is contained in $B$ and $B$ contains $A$ are alternative ways of saying that $A$ is a subset of $B$</em>

$A \nsubseteq B \quad$ means that $\quad$ there is at least one element $x$ such that $x \in A$ and $x \notin B$

If $A$ = &#123;1, 2&#125; and $B$ = &#123;&#123;1, 2&#125;, 3&#125;, then $1 \in A$, $1 \notin B$, $A \in B$, $A \nsubseteq B$
<ul>
  <li>
  
  The cardinality of $B$ = &#123;&#123;1, 2&#125;, 3&#125; is 2, not 3, since there are two elements of $B$: the set &#123;1, 2&#125; and the number 3</li>
  <li>The numbers 1 and 2 are not elements of $B$; instead, they are elements of a set contained in $B$</li>
</ul>  

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>Is $2 \in$ &#123;1, 2, 3&#125;</li>
  <li>Is &#123;3&#125; $\subseteq$ &#123;3&#125;</li>
  <li>Is &#123;1, 2&#125; $\in$ &#123;1, 2, 3&#125;</li>
  <li>Is &#123;2&#125; $\in$ &#123;&#123;1&#125;, &#123;2&#125;, &#123;3&#125;&#125;</li>
  <li>Is $1 \in$ &#123;&#123;1&#125;, 2, 3&#125;</li>
  <li>Is &#123;2&#125; $\in$ &#123;1, 2, 3&#125;</li>
  <li>Is $&#123;1, 3&#125; \subseteq &#123;1, 2, 3&#125;</li>
  <li>Is $2 \in$ &#123;&#123;1&#125;, &#123;2&#125;, &#123;3&#125;&#125;</li>
  <li>Is &#123;3&#125; $\subseteq$ &#123;1, 2, 3&#125;</li>
  <li>Is $2 \in$ &#123;&#123;2&#125;, 3&#125;</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>
<ol type="a">
  <li>Yes, the element 2 is indeed in the set</li>
  <li>Yes, 3&#125; is a subset of itself because all of the elements in the set, 3, are within itself</li>
  <li>No, &#123;1, 2&#125;$ is a set and there is no element in &#123;1, 2, 3&#125; that is a set</li>
  <li>Yes, &#123;2&#125;$ is an element in the set since there an element in the set which contains the &#123;2&#125; set</li>
  <li>No, 1 is not an element in the set. An element of the set is &#123;1&#125;, not 1</li>
  <li>Yes, &#123;2&#125; is a subset of the set</li>
  <li>Yes, both elements in this set, &#123;1, 3&#125;, can be found in this set, &#123;1, 2, 3&#125;</li>
  <li>No, 2 is not an element of the set since the elements of the set are other sets</li>
  <li>Yes, &#123;3&#125; is a subset of the set since the set &#123;3&#125; is a subset of the larger set, since the large set has an element with the value 3</li>
  <li>No, 2 is not an element of the set; however, &#123;2&#125; is an element of the set</li>
</ol>
</details>
</ul>  
</details>

### Empty Sets
An <strong>empty set</strong> is denoted by $\emptyset$ or &#123;&#125;

A set $A$ is called an empty set if its cardinality is 0, meaning:

<div align="center">

$A = \emptyset \quad$ if and only if $\quad x \notin A$
</div>

This means that no element $x$ exists such that $x$ is a member of $A$

The empty set is a subset of every set, including itself:

<div align="center">

$\emptyset \subseteq A \quad$ for any set $\quad A$
</div>

### Equal Sets
Two sets are <strong>equal</strong> if they contain exactly the same things

More precisely, $A = B$ if $A \subseteq B$ and $B \subseteq A$, meaning that every element of $A$ is an element of $B$ and every element of $B$ is an element of $A$

### Cartesian Product
Given elements $a$ and $b$, the symbol $(a, b)$ denotes the <strong>ordered pair</strong> consisting of $a$ and $b$ together with the specification that $a$ is the first element of the pair and $b$ is the second element

Two ordered pairs $(a, b)$ and $(c, d)$ are equal if, and only if, $a = c$ and $b = d$

Given sets $A$ and $B$, the <strong>Cartesian product of $A$ and $B$</strong> denoted <strong>$A$ x $B$</strong> and read $A$ cross $B$, is the set of all ordered pairs $(a, b)$ where $a$ is in $A$ and $b$ is in $B$

<details>
    <summary>Example problem</summary>

Let $A$ = &#123;1, 2, 3&#125; and $B$ = &#123;u, v&#125;
<ol type="a">
  <li>Find $A$ x $B$</li> 
  <li>Find $B$ x $B$</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>
<ol type="a">
  <li>$A$ x $B$ = &#123;(1, u), (2, u), (3, u), (1, v), (2, v), (3, v)&#125;</li>
  <li>$B$ x $B$ = &#123;(u, u), (v, u), (v, u), (v, v)&#125;</li>
</ol>  
</details>
</ul>  
</details>

## The Language of Relations and Functions
Let $A$ and $B$ be sets. A <strong>relation</strong> from $A$ to $B$ is a subset $R$ of $A$ x $B$. if $x \in A$ is related to $y \in B$:

<div align="center">

$x R y \quad$ or equivalently $\quad (x, y) \in R$
</div>

If $x$ is not related to $y$:

<div align="center">

$x \cancel{R} y \quad$ or equivalently $\quad (x, y) \notin R$
</div>

The set $A$ is called the <strong>domain</strong> of $R$ and the set of $B$ is called the <strong>co-domain</strong> of $R$

A relation is a <strong>function</strong> from $A$ to $B$ if every element of $A$ is related to exactly one element of $B$

<details>
    <summary>Example problem</summary>

Let $A$ = &#123;0, 1, 2&#125; and $B$ = &#123;1, 2, 3&#125; and let's say that an element $x$ in $A$ is related to an element $y$ in $B$ if, and only if, $x$ is less than $y$. Use the notation $x R y$ as a shorthand for the sentence $x$ is related to $y$
<ul>  
  <details>
    <summary>Solution</summary>

0 $R$ 1 $\quad$ since $\quad$ 0 < 1<br />
0 $R$ 2 $\quad$ since $\quad$ 0 < 2<br />
0 $R$ 3 $\quad$ since $\quad$ 0 < 3<br />
1 $\cancel{R}$ 1 $\quad$ since $\quad$ 1 $\cancel{<}$ 1<br />
1 $R$ 2 $\quad$ since $\quad$ 1 < 2<br />
1 $R$ 3 $\quad$ since $\quad$ 1 < 3<br />
2 $\cancel{R}$ 1 $\quad$ since $\quad$ 2 $\cancel{<}$ 1<br />
2 $\cancel{R}$ 2 $\quad$ since $\quad$ 2 $\cancel{<}$ 2<br />
2 $R$ 3 $\quad$ since $\quad$ 2 < 3<br /><br />

$R$ = &#123;(0, 1), (0, 2), (0, 3), (1, 2), (1, 3), (2, 3)&#125;
</details>
</ul>  
</details>

The notation for a relation $R$ may be written symbolically as follows:
<div align="center">

$x R y \quad$ means that $\quad (x, y) \in R$
</div>

The notation $x \cancel{R} y$ means that $x$ is not related to $y$ by $R$:
<div align="center">

$x \cancel{R} y \quad$ means that $\quad (x, y) \notin R$
</div>

<details>
    <summary>Example problem</summary>

Let $C = D$ = &#123;-3, -2, -1, 1, 2, 3&#125; and define a relation $S$ from $C$ to $D$ as follows

<div align="center">

For every $(x, y) \in C$ x $D, (x, y) \in S$ means that $1/x - 1/y$ is an integer
</div>
<ol type="a">
  <li>
  
  Is $2 S 2$<br />
  Is $-1 S -1$<br />
  Is $(3, 3) \in S$<br />
  Is $(3, -3) \in S$</li>
  <li>Write $S$ as a set of ordered pairs</li>
  <li>What is the domain of $S$<br />
  What is the co-domain of $S$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $1/2 - 1/2 = 0$, which is an integer. So $2 R 2$<br />
  $-1/2 + 1/2 = 0$, which is an integer. So $-1 R -1$<br />
  $1/3 - 1/3 = 0$, which is an integer. So $(3, 3) \in S$<br />
  $1/3 + 1/3 = 2/3$, which is not an integer. So $(3, -3) \in S$</li>
  <li>
  
  $S$ = &#123;(-3, -3), (-2, -2), (-2, 2), (-1, -1), (-1, 1), (1, -1). (1, 1), (2, -2), (2, 2), (3, 3&#125;</li>
  <li>

  domain of $S$ = &#123;-3, -2, -1, 1, 2, 3&#125;<br />
  co-domain of $S$ = &#123;-3, -2, -1, 1, 2, 3&#125;</li>
</ol>  
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $G$ = &#123;-2, 0, 2&#125; and $H$ = &#123;4, 6, 8&#125; and define a relation $V$ from $G$ to $H$ as follows

<div align="center">

For every $(x, y) \in G$ x $H, (x, y) \in V$ means that $(x - y)/ 4$ is an integer
</div>
<ol type="a">
  <li>
  
  Is $2 V 6$<br />
  Is $-2 V 8$<br />
  Is $(0, 6) \in V$<br />
  Is $(2, 4) \in V$</li>
  <li>Write $S$ as a set of ordered pairs</li>
  <li>What is the domain of $V$<br />
  What is the co-domain of $V$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $(2 - 6) / 4 = -1$, which is an integer. So $2 V 6$<br />
  $(-2 - 8) / 4 = -10/4$, which is not an integer. So $-2 \cancel{V} 8$<br />
  $(0 - 6) / 4 = -6/4$, which is not an integer. So $(0, 6) \notin V$<br />
  $(2 - 4) / 4 = -2/4$, which is not an integer. So $(2, 4) \notin V$</li>
  <li>
  
  $V$ = &#123;(-2, 6), (0, 4), (0, 8), (2, 6)&#125;</li>
  <li>

  domain of $V$ = &#123;-2, 0, 2&#125;<br />
  co-domain of $V$ = &#123;4, 6, 8&#125;</li>
</ol>  
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Define a relation $S$ from <strong>$R$</strong> to <strong>$R$</strong> as follows:

<div align="center">

For every $(x, y) \in $<strong>$R$</strong> x <strong>$R$</strong>$, (x, y) \in S$ means that $x \geq y$
</div>
<ol type="a">
  <li>
  
  Is $(9, 8) \in S$<br />
  Is $(9, 9) \in S$<br />
  Is $9 S 10$<br />
  Is $(-1) S (-2)$</li>
  <li>Write $S$ as a set of ordered pairs</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $9 \geq 8$, so $(9, 8) \in S$<br />
  $9 \geq 9$, so $(9, 9) \in S$<br />
  $9 \cancel{\geq} 8$, so $9 \cancel{S} 10$<br />
  $-1 \geq -2$, so $(-1) S (-2)$</li>
</ol>  
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Define a relation $R$ from <strong>$R$</strong> to <strong>$R$</strong> as follows:

<div align="center">

For every $(x, y) \in $<strong>$R$</strong> x <strong>$R$</strong>$, (x, y) \in S$ means that $y = x$<sup>2</sup>
</div>
<ol type="a">
  <li>
  
  Is $(6, 36) \in R$<br />
  Is $(36, 6) \in R$<br />
  Is $(-5) R 25$<br />
  Is $25 R (-5)$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $36 = 6^2$, so $(6, 36) \in R$<br />
  $6 \cancel{=} 36^2$, so $(36, 6) \notin R$<br />
  $25=(-5)^2$, so $(-5) R 25$<br />
  $-5 \cancel{=} 25^2$, so $25 \cancel{R} (-5)$</li>
</ol>  
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $A$ = &#123;2, 4&#125; and $B$ = &#123;1, 3, 5&#125; and define relations $U$, $V$, and $W$ from $A$ to $B$ as follows:

<div align="center">

For every $(x, y) \in A$ x $B$<br />
$(x, y) \in U$ means that $y - x > 2$,<br />
$(x, y) \in V$ means that $y - 1 = x/2$, and<br />
$W$ = &#123;(2, 5), (4, 1), (2, 3)&#125;
</div>
<ul>  
  <details>
    <summary>Solution</summary>

$U$ = &#123;(2, 5)&#125;
$V$ = &#123;(4, 3)&#125;
</details>
</ul>  
</details>
