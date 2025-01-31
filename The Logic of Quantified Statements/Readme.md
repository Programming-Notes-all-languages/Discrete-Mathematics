<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#predicates-and-quantified-statements'>Predicates and Quantified Statements</a>
  </li>
</ol>
</details>

## Predicates and Quantified Statements
A <strong>predicate</strong>is a sentence that contains a finite number of variables and becomes a statement when specific values are substituted for the variables

The <strong>domain</strong> of a predicate variable is the set of all values that may be substituted in place of the variable

<details>
    <summary>Example problem</summary>

Let $P(x)$ be the predicate $x$<sup>2</sup> $> x$ with the domain the set of $\mathbb{R}$ of all real numbers. Write $P(2)$, $P(1/2)$, and $P(-1/2)$, and indicate which of these statements are true and which are false
<ul>  
  <details>
    <summary>Solution</summary>

$P(2): 2$<sup>2</sup> $ > 2$ which is true<br />
$P(1/2): (1/2)$<sup>2</sup> $> 1/2$ which is false<br />
$P(-1/2): (-1/2)$<sup>2</sup> which is true
</details>
</ul>  
</details>

If $P(x)$ is a predicate and $x$ has the domain $D$, the <strong>truth set</strong> of $P(x)$ is the set of all elements of $D$ that make $P(x)$ true when they are substituted for $x$. The truth set of $P(x)$ is denoted

<div align="center">

&#123; $x$ $\in$ $D$ $|$ $P$ $($ $x$ $)$&#125;
</div>

<details>
    <summary>Example problem</summary>

Let $Q(n)$ be the predicate $n$ is a factor of 8. Find the truth set of $Q(n)$ if
<ol type="a">
  <li>

  The domain of $n$ is the set $\mathbb{Z}^+$ of all positive integers</li>
  <li>

  The domain of $n$ is the set $\mathbb{Z}$ of all integers</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
The truth set is &#123;$1, 2, 4, 8$&#125;</li>
<li>

The truth set is &#123;$1, 2, 4, 8, -1, -2, -4, -8$&#125;</li>
</ol>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $Q(x, y)$ be the predicate, if $x < y$ than $x$<sup>2</sup> $< y$<sup>2</sup>, with domain for both $x$ and $y$ being $\mathbb{R}$, the set of all real numbers 
<ol type="a">
  <li>

  When $x = -2$ and $y = 1$, is $Q(x, y)$ true or false?</li>
  <li>

  Give values different from those in part a for which $Q(x, y)$ has the same truth value as in part a</li>
  <li>

  When $x = 3$ and $y = 8$, is $Q(x, y)$ true or false?</li>
  <li>

  Give values different from those in part c for which $Q(x, y)$ has the same truth value as in part c</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  The hypothesis $Q(-2, 1)$ is $-2 < 1$, which is true. The conclusion is $4 < 1$, which is false. Thus, $Q(-2, 1)$ is a conditional statement with a true hypothesis and a false conclusion. So $Q(-2, 1)$ is false</li>
  <li>

  $(x, y) = (-3, 1)$</li>
  <li>

  The hypothesis of $Q(3, 8)$ is $3 < 8$, which is true. The conclusion is $9 < 64$, which is true. Thus $Q(3, 8)$ is a conditional statement with a true hypothesis and a true conclusion. So $Q(3, 8)$ is true</li>
  <li>

  $(x, y) = (4, 6)$</li>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Find the truth set of each predicate
<ol type="a">
  <li>

  Predicate: $8/d$ is an integer, domain: $\mathbb{Z}$</li>
  <li>

  Predicate: $8/d$ is an integer, domain: $\mathbb{Z}$<sup>+</sup></li>
  <li>

  Predicate: $1 \leq x$<sup>2</sup> $ \leq 4$, domain: $\mathbb{R}$</li>
  <li>

  Predicate: $1 \leq x$<sup>2</sup> $\leq 4$, domain: $\mathbb{Z}$</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  &#123;$-8, -4, -2, -1, 1, 2, 4, 8$&#125;</li>
  <li>

  &#123;$1, 2, 4, 8$&#125;</li>
  <li>

  $1 \leq x$<sup>2</sup> is true when $x \geq 1$ or when $x \leq -1$<br />
  $x$<sup>2</sup> $\leq 4$ is true when $x \leq 2$ and $x \geq -2$<br /><br />
  $[-2, -1]$ or $[1, 2]$ </li>
  <li>

  &#123;$-2, -1, 1, 2$&#125;</li>
</details>
</ul>  
</details>

### The Universal Quantifier: $\forall$
<strong>Quantifiers</strong> are words that refer to quantities such as some or all and tell for how many elements a given predicate is true

The $\forall$ symbol denotes for all and is called the <strong>universal quantifier</strong>

For example, another way to express the sentence, all human beings are moral, is to write

<div align="center">

$\forall$ human beings $x$, $x$ is mortal
</div>

Let $Q(x)$ be a predicate and $D$ the domain of $x$. A <strong>universal statement</strong> is a statement of the form, $\forall x \in D, Q(x)$. It is defined to be true if, and only if, $Q(x)$ is true for every $x$ in $D$. It is defined to be false if, and only if, $Q(x)$ is false for at least one in $x$ in $D$. A value for $x$ for which $Q(x)$ is false is called a <strong>counterexample</strong> to the universal statement

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>
  
  Let $D =$ &#123; $1, 2, 3, 4, 5$ &#125;, and consider the statement

<div align="center">

$\forall$ $x$ $\in$ $D$ $,$ $x$<sup>2</sup> $\geq$ $x$
</div>
  Show that this statement is true</li>
  <li>Consider the statement

<div align="center">

$\forall$ $x$ $\in$ $\mathbb{R}$, $x$<sup>2</sup> $\geq$ $x$
</div>
  Find a counterexample to show that this statement is false</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $1$<sup>2</sup> $\geq 1$ is true<br />
  $2$<sup>2</sup> $\geq 2$ is true<br />
  $3$<sup>2</sup> $\geq 3$ is true<br />
  $4$<sup>2</sup> $\geq 4$ is true<br />
  $5$<sup>2</sup> $\geq 5$ is true<br /><br />
  Hence, $\forall x \in D, x$<sup>2</sup> $\geq x$</li>
  <li>
  
  Take $x = 1/2$<br />
  $(1/2)$<sup>2</sup> = $1/4$ $\cancel{\geq}$ 1/2<br /><br />
  Hence, $\forall x \in \mathbb{R}, x$<sup>2</sup> $\geq x$ is false</li>
</ol>  
</details>
</ul>  
</details>

### The Existential Quantifier: $\exists$
The symbol $\exists$ denotes there exists and is called the <strong>existential quantifier</strong>

For example, the sentence, there is a student in Math 140, can be written as

<div align="center">

$\exists$ a person $p$ such that $p$ is a student in Math 140
</div>

Let $Q(x)$ be a predicate and $D$ the domain of $x$. An <strong>existential statement</strong> is a statement of the form $\exists x \in D$ such that $Q(x)$. It is defined to be true if, and only if, $Q(x)$ is true for at least one $x$ in $D$. It is false if, and only if, $Q(x)$ is false for all $x$ in $D$

<details>
    <summary>Example problem</summary>

<ol type="a">
  <li>Consider the statement

<div align="center">

$\exists$ $m$ $\in$ $\mathbb{Z}$<sup>+</sup> such that $m$<sup>2</sup> $=$ $m$
</div>
  Show that this statement is true</li>
  <li>

  Let $E = $ &#123; $5, 6, 7, 8$ &#125; and consider the statement

<div align="center">

$\exists$ $m$ $\in$ $E$ such that $m$<sup>2</sup> $=$ $m$
</div>
  Show that this statement is false</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  For $m = 1$, $1$<sup>2</sup> $= 1$ which is true for at least one integer; therefore, the statement is true</li>
  <li>
  
  For $m = 5, 6, 7, 8$, none of these integers squared equal the integer itself</li>
</ol>  
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $D$ be the set of all students at your school, and let $M(s)$ be, $s$ is a math major, let $C(s)$ be, $s$ is a computer science student, and let $E(s)$ be, $s$ is an engineering student. Express each of the following statements using quantifiers, variables, and the predicates $M(s)$, $C(s)$, and $E(s)$
<ol type="a">
  <li>There is an engineering student who is a math major</li>
  <li>Every computer science student is an engineering student</li>
  <li>No computer science students are engineering students</li>
  <li>Some computer science students are also math majors</li>
  <li>Some computer science students are engineering students and some are not</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $\exists s \in D$ such that $E(s) \land M(s)$</li>
  <li>

  $\forall s \in D, C(s) \rightarrow E(s)$</li>
  <li>

  $\forall s \in D, C(s) \rightarrow \neg E(s)$</li>
  <li>

  $\exists s \in D$ such that $C(s) \land M(s)$</li>
  <li>

  $\exists s \in D$ such that $C(s) \land E(s) \land (\exists s \in D$ such that $C(s) \land \neg E(s))$</li>
</ol>  
</details>
</ul>  
</details>

### Negation of a Universal Statement
The negation of $\forall x P(x)$ is $\exists x \neg P(x)$

<div align="center">

$\neg$ $($ $\forall$ $x$ $P$ $($ $x$ $)$ $)$ $\equiv$ $\exists$ $x$ $\neg$ $P$ $($ $x$ $)$</div>

Symbolically, $\quad \neg (\forall x \in D, P(x)) \equiv \exists x \in D$ such that $\neg P(x)$

<details>
    <summary>Example problem</summary>

Consider the following statement

<div align="center">

$\forall$ $n$ $\in$ $\mathbb{Z}$ $,$ if $n$ is prime then $n$ is odd or $n$ $=$ $2$</div>

Write the negation of the statement above
<ul>  
  <details>
    <summary>Solution</summary>

Solving for $\quad \neg (\forall n \in \mathbb{Z},$ if $n$ is prime then $n$ is odd or $n = 2)$<br />
If $n$ is prime then $n$ is odd or $n = 2$ = $p \rightarrow q \vee r$<br />
$\quad \quad p \land \neg(q \vee r)$<br />
$\quad \quad p \land (\neg q \land \neg r)$<br /><br />
$\exists n \in \mathbb{Z},$ such that $n$ is prime and $n$ is not odd and $n$ is not equal to 2
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Consider the following statement

<div align="center">

$\forall$ integer, if $n$ is divisible by 6, then $n$ is divisible by 2 and $n$ is divisible by 3</div>

Write the negation of the statement above
<ul>  
  <details>
    <summary>Solution</summary>

Solving for $\forall$ integer, if $n$ is divisible by 6, then $n$ is divisible by 2 and $n$ is divisible by 3<br />
If $n$ is divisible by 6, then $n$ is divisible by 2 and $n$ is divisible by 3 = $p \rightarrow q \land r$<br />
$\quad \quad p \land \neg(q \land r)$<br />
$\quad \quad p \land (\neg q \vee \neg r)$<br /><br />
$\exists$ an integer $n$ such that $n$ is divisible by 6 and $n$ is not divisive by 2 or $n$ is not divisible by 3
</details>
</ul>  
</details>

### Negation of an Existential Statement
The negation of $\neg(\exists x \in D, P(x))$ is  $\forall x \in D, \neg P(x)$

<div align="center">

$\neg$ $($ $\exists$ $x$ $\in$ $D$, $P$ $($ $x$ $)$ $)$ $\equiv$ $\forall$ $x$ $\in$ $D$, $\neg$ $P$ $($ $x$ $)$</div>

Symbolically, $\quad \neg(\exists x \in D$ such that $P(x)) \equiv \forall x \in D, \neg P(x)$

<details>
    <summary>Example problem</summary>

Consider the following statement
<div align="center">

$\forall$ $a$ $\in$ $\mathbb{Z}$ $,$ $($ $a$ $-$ $1$ $)$ $/$ $a$ is not an integer</div>

<ol type="a">
  <li>Write the negation of the statement above</li>
  <li>
  
  Is the given statement true or false? If the statement is true, enter TRUE; if the statement is false, enter a value of $a$ that could be used as part of a counterexample that justifies its falseness</li>
<ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>There is an integer $a$ such that $($ $a$ $-$ $1$ $)$ $/$ $a$ is an integer</li>
  <li>1</li>
<ol>  
</details>
</ul>  
</details>

### The Relation among $\forall$, $\exists$, $\land$, and $\vee$
If $Q(x)$ is a predicate and the domain $D$ if $x$ is the set &#123;$x$<sub>1</sub>$, x$<sub>2</sub>$, ...x$<sub>n</sub>&#125;, then the statements

<div align="center">

$\forall$ $x$ $\in$ $D$ $,$ $Q$ $($ $x$ $)$<br />
and $Q$ $($ $x$<sub>1</sub> $)$ $\land$ $Q$ $($ $x$<sub>2</sub> $)$ $\land$ $.$ $.$ $.$ $\land$ $Q$ $($ $x$<sub>n</sub> $)$</div>

are logically equivalent

Let $P(x)$ and $Q(x)$ be predicates and suppose the common domain of $x$ is $D$
<ul>
  <li>
  
  The notation $P(x) \rightarrow Q(x)$ means that every element in the truth set of $P(x)$ is in the truth set of $Q(x)$</li>
  <li>

  The notation $P(x) \leftrightarrow Q(x)$ means that $P(x)$ and $Q(x)$ have identical truth sets</li>
</ul>  

### Vacuous Truth of Universal Statements
A statement is <strong>vacuously true</strong> when it has the logical form of an implication $(P \rightarrow Q)$, but the hypothesis $P$ is always false

In other words, a statement of the form

<div align="center">


$\forall$ $x$ $\in$ $D$ $,$ $P$ $($ $x$ $)$ $\rightarrow$ $Q$ $($ $x$ $)$</div>

is vacuously true if there are no elements in $D$ for which $P(x)$ is true

### Variants of Universal Conditional Statements
Consider a statement of the form: $\quad \forall x \in D,$ if $P(x)$ then $Q(x)$
<ol>
  <li>

  Its <strong>contrapositive</strong> is the statement: $\quad \forall x \in D,$ if $\neg Q(x)$ then $\neg P(x)$</li>
  <li>

  Its <strong>converse</strong> is the statement: $\quad \forall x \in D,$ if $Q(x)$ then $P(x)$</li>
  <li>

  Its <strong>inverse</strong> is the statement: $\quad \forall x \in D,$ if $\neg P(x)$ then $\neg Q(x)$</li>
</ol>

<details>
    <summary>Example problem</summary>

Consider the following statement
<div align="center">

If $n$ is any prime number that is greater than $2$, then $n + 1$ is even</div>

Write the converse of the statement and give a counterexample to show that the converse is false
<ul>  
  <details>
    <summary>Solution</summary>

If $n$ is any prime number that is greater than $2$, then $n + 1$ is even = $p \rightarrow q$<br /><br />
If $n + 1$ is even, then $n$ is any prime number that is greater than $2$<br />
A counterexample is if $n = 9$
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Consider the following statement
<div align="center">

$\forall$ integer $d$, if $6$ $/$ $d$ is an integer, then $d$ $=$ $3$</div>

<ol type="a">
  <li>Write the contrapositive of the statement and determine if the contrapositive is true or false</li>
  <li>Write the converse of the statement and determine if the converse is true or false</li>
  <li>Write the inverse of the statement and determine if the inverse is true or false</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  $\forall$ integer $d$, if $d \cancel{=} 3$, then $6 / d$ is not an integer<br />
  A counterexample is when $d = 2$</li>
  <li>

  $\forall$ integer $d$, if $d = 3$, then $6 / d$ is an integer<br />
  The converse is true</li>
  <li>

  $\forall$ integer $d$, if $6 / d$ is not an integer, then $d \cancel{=} 3$<br />
  The inverse is true</li>
</ol>  
</details>
</ul>  
</details>

### Necessary and Sufficient Conditions, Only If
<ul>
  <li>

  $\forall x, r(x)$ is a <strong>sufficient condition</strong> for $s(x)$ means $\forall x,$ if $r(x)$ then $s(x)$</li>
  <li>

  $\forall x, r(x)$ is a <strong>necessary condition</strong> for $s(x)$ means $\forall x,$ if $\neg r(x)$ then $\neg s(x)$</li>
  <li>

  $\forall x, r(x)$ <strong>only if</strong> $s(x)$ means $\forall x,$ if $\neg s(x)$ then $\neg r(x)$ or equivalently $\forall x,$ if $r(x)$ then $s(x)$</li>
