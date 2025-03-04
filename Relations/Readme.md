<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#relations-on-sets'>Relations on Sets</a>
  </li>
  <li>
    <a href='#reflexivity-symmetry-and-transitivity'>Reflexivity, Symmetry, and Transitivity</a>
  </li>
  <li>
    <a href='#equivalence-relations'>Equivalence Relations</a>
  </li>
</ol>
</details>

## Relations on Sets
Let $A$ and $B$ be sets. A <strong>relation</strong> from $A$ to $B$ is a subset $R$ of $A$ x $B$. if $x \in A$ is related to $y \in B$:

<div align="center">

$x$ $R$ $y$ $\quad$ or equivalently $\quad$ $($ $x$, $y$ $)$ $\in$ $R$
</div>

If $x$ is not related to $y$:

<div align="center">

$x \cancel{R} y$ $\quad$ or equivalently $\quad$ $($ $x$, $y$ $)$ $\notin$ $R$
</div>

The set $A$ is called the <strong>domain</strong> of $R$ and the set of $B$ is called the <strong>co-domain</strong> of $R$

A relation is a <strong>function</strong> from $A$ to $B$ if every element of $A$ is related to exactly one element of $B$

<details>
    <summary>Example problem</summary>

Let $A$ = {$-3, 0, 3$} and $B$ = {$t, u, v, w$}. Define a function $F$: $A \rightarrow B$ by the following arrow diagram

<ol type="a">
  <li>
  
  What are the domain and co-domain of $F$?</li>
  <li>

  What is $F(-3), F(0), F(3)$?
</ol>

<img src="Images/Example Problems/Problem 1.png" alt="Problem 1">
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>
  
  Domain of $F = ${$-3, 0, 3$}<br />
  Co-domain of $F = ${$t, u, v, w$}</li>
  <li>

  $F(-3) = u$<br />
  $F(0) = w$<br />
  $F(3) = u$</li>
</details>
</ul>  
</details>

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

$x$ $R$ $y$ $\quad$ means that $\quad$ $($ $x$, $y$ $)$ $\in$ $R$
</div>

The notation $x \cancel{R} y$ means that $x$ is not related to $y$ by $R$:
<div align="center">

$x \cancel{R} y$ $\quad$ means that $\quad$ $($ $x$, $y$ $)$ $\notin$ $R$
</div>

<details>
    <summary>Example problem</summary>

Let $C = D$ = &#123;-3, -2, -1, 1, 2, 3&#125; and define a relation $S$ from $C$ to $D$ as follows

<div align="center">

For every $($ $x$, $y$ $)$ $\in$ $C$ x $D$, $($ $x$, $y$ $)$ $\in$ $S$ means that $1$ $/$ $x$ $-$ $1$ $/$ $y$ is an integer
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
  
  $1/2 - 1/2 = 0$, which is an integer. So $2 S 2$<br />
  $-1/2 + 1/2 = 0$, which is an integer. So $-1 S -1$<br />
  $1/3 - 1/3 = 0$, which is an integer. So $(3, 3) \in S$<br />
  $1/3 + 1/3 = 2/3$, which is not an integer. So $(3, -3) \in S$</li>
  <li>
  
  $S$ = &#123;(-3, -3), (-2, -2), (-2, 2), (-1, -1), (-1, 1), (1, -1). (1, 1), (2, -2), (2, 2), (3, 3)&#125;</li>
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

For every $($ $x$, $y$ $)$ $\in$ $G$ x $H$, $($ $x$, $y$ $)$ $\in$ $V$ means that $($ $x$ $-$ $y$ $)$ $/$ $4$ is an integer
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

For every $($ $x$, $y$ $)$ $\in$ <strong>$R$</strong> x <strong>$R$</strong>, $($ $x$, $y$ $)$ $\in$ $S$ means that $x$ $\geq$ $y$
</div>

Is $(9, 8) \in S$<br />
  Is $(9, 9) \in S$<br />
  Is $9 S 10$<br />
  Is $(-1) S (-2)$</li>
<ul>  
  <details>
    <summary>Solution</summary>

$9 \geq 8$, so $(9, 8) \in S$<br />
  $9 \geq 9$, so $(9, 9) \in S$<br />
  $9 \cancel{\geq} 8$, so $9 \cancel{S} 10$<br />
  $-1 \geq -2$, so $(-1) S (-2)$
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Define a relation $R$ from <strong>$R$</strong> to <strong>$R$</strong> as follows:

<div align="center">

For every $($ $x$, $y$ $)$ $\in$ <strong>$R$</strong> x <strong>$R$</strong>, $($ $x$, $y$ $)$ $\in$ $S$ means that $y$ $=$ $x$<sup>2</sup>
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

For every $(x, y) \in A$ x $B$<br />
$(x, y) \in U$ means that $y - x > 2$,<br />
$(x, y) \in V$ means that $y - 1 = x/2$, and<br />
$W$ = &#123;(2, 5), (4, 1), (2, 3)&#125;
<ul>  
  <details>
    <summary>Solution</summary>

$U$ = &#123;(2, 5)&#125;
$V$ = &#123;(4, 3)&#125;
</details>
</ul>  
</details>

### The Inverse of a Relation
If $R$ is a relation from $A$ 5o $B$, then a relation $R$<sup>-1</sup> from $B$ to $A$ can be defined by interchanging the elements of all ordered pairs of $R$

<details>
    <summary>Example problem</summary>

Let $A$ = &#123;2, 3, 4&#125; and $B$ = &#123;2, 6, 8&#125; and let $R$ be the divides relation from $A$ and $B$: For all $(x, y) \in A x B$,

<div align="center">

$x$ $R$ $y$ $\iff$ $x$ $|$ $y$
</div>

State explicitly which ordered pairs are in $R$ and $R$<sup>-1</sup>, and draw arrow diagrams for $R$ and $R$<sup>-1</sup>
</div>

<ul>  
  <details>
    <summary>Solution</summary>

$R =$ &#123;$(2, 2), (2, 6), (2, 8), (3, 6), (4, 8)$ &#123;<br />
$R$<sup>-1</sup> $ = (2, 2), (6, 2), (8, 2), (6, 3), (8, 4)$

<img src="Images/Example Problems/Problem 2A.png" alt="Problem 2A">
</details>
</ul>  
</details>

## Reflexivity, Symmetry, and Transitivity
Let $R$ be a relation on a set $A$
<ol>
  <li>

  $R$ is <strong>reflexive</strong> if, and only if, for all $x \in A, x R x$</li>
  <li>

  $R$ is <strong>symmetric</strong> if, and only if, for all $x, y \in A$, if $x R y$ then $y R x$</li>
  <li>

  $R$ is <strong>transitive</strong> if, and only if, for all $x, y, z \in A$, if $x R y$ and $y R z$ then $x R z$</li>
</ol>

In informal terms:
<ol>
  <li><strong>Reflexive</strong>: each element is related to itself</li>
  <li><strong>Symmetric</strong>: if any one element is related to any other element, then the second element is related to the first</li>
  <li><strong>Transitive</strong>: if any one element is related to a second and that second element is related to a third, then the first element is related to the third</li>
</ol>

Now considering what is means for a relation not to have one of the properties defined previously. Hence if $R$ is a relation on a set $A$, then
<ol>
  <li>
  
  $R$ is <strong>not reflexive</strong> $\iff$ there is an element $x$ in $A$ such that $x \cancel{R} x$</li>
  <li>

  $R$ is <strong>not symmetric</strong> $\iff$ there are elements $x$ and $y$ in $A$ such that $x R y$ but $y \cancel{R} x$</li>
  <li>

  $R$ is <strong>not transitive</strong> $\iff$ there are elements $x, y,$ and $z$ in $A$ such that $x R y$ and $y R z$ but $x \cancel{R} z$</li>
</ol>  

<details>
    <summary>Example problem</summary>

Let $A = {0, 1, 2, 3}$, and define a relation $R$<sub>2</sub> on $A$ as follows: $R$<sub>2</sub> $ = \{(0, 0), (0, 1), (1, 1), (1, 2), (2, 2), (2, 3)\}$

<ol type="a">
  <li>

  Draw the directed graph of $R$<sub>2</sub></li>
  <li>

  Is $R$<sub>2</sub> reflexive?</li>
  <li>

  Is $R$<sub>2</sub> symmetric?</li>
  <li>

  Is $R$<sub>2</sub> transitive?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  <img src="Images/Example Problems/Problem 3A.png" alt="Problem 3A"></li>
  <li>

  $R$<sub>2</sub> is not reflexive because when $m = 3$, then $(m, m) \notin$ $R$<sub>2</sub></li>
  <li>

  $R$<sub>2</sub> is not symmetric because $(1, 2) \in$ $R$<sub>2</sub> and $(2, 1) \notin$ $R$<sub>2</sub></li>
  <li>

  $R$<sub>2</sub> is not transitive because $(0, 1) \in$ $R$<sub>2</sub> and $(1, 2) \in$ $R$<sub>2</sub>, and $(0, 2) \notin$ $R$<sub>2</sub></li>
</ol>
</details>
</ul>  
</details>

To disprove reflexivity, find one $x$ where $x R x$ fails. Reflexivity must hold for all $x$ in the domain

To disprove symmetry, find $x$, $y$ where $x R y$ holds but $y R x$ does not. Symmetry must hold for only pairs in the relation

To disprove transitivity, find three numbers $x, y, z$ such that $x R y$ and $y R z$ hold, but $x R z$ fails. For transitivity to hold, if $x R y$ and $y R z$, then $x R z$ must hold for all $x, y, z$

<details>
    <summary>Example problem</summary>

Let $C$ be the circle relation defined on the set of real numbers

<div align="center">

For every $x$, $y$ $\in$ $\mathbb{R}$, $x$ $C$ $y$ $\iff$ $x$<sup>2</sup> $+$ $y$<sup>2</sup> $=$ $1$
</div>

<ol type="a">
  <li>

  Is $C$ reflexive?</li>
  <li>

  Is $C$ symmetric?</li>
  <li>

  Is $C$ transitive?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $C$ is not reflexive because for a relation to be reflexive, $x C x$ meaning $x$<sup>2</sup> $+ x$<sup>2</sup> $ = 1$. This means $2x$<sup>2</sup> $ = 1$ which means that this is only true when $x$ = -1/2 and +1/2. However, $x \in R$ so when $x$ = 3, the case is false since 18 does not equal 1; therefore, $C$ is not reflexive</li>
  <li>

  $C$ is symmetric because for all pairs of the relation, reversing $x$ and $y$ still results in the relation holding</li>
  <li> 

  $C$ is not transitive because when $x, y, z = (-1, 0, 1)$, $x C y$, $y C z$, but $x \cancel{C} z$</li>
</ol>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $O$ be the relation defined on $\mathbb{Z}$ as follows

<div align="center">

For every $m$, $n$ $\in$ $\mathbb{Z}$, $m$ $O$ $n$ $\iff$ $m$ $-$ $n$ is odd
</div>

<ol type="a">
  <li>

  Is $O$ reflexive?</li>
  <li>

  Is $O$ symmetric?</li>
  <li>

  Is $O$ transitive?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $O$ is not reflexive because when $m = 1$, then $m - m$ is not odd</li>
  <li>

  $O$ is symmetric because for all pairs of the relation, reversing $m$ and $n$ still results in the relation holding</li>
  <li> 

  Suppose $m = 8$, $m O n$ holds when $m = 8$ and $n = 3$. Then, $m O n$ holds when $n = 3$ and $o = 2$. However, $m \cancel{O} n$ when $m = 8$ and $o = 2$; therefore, $O$ is not transitive</li>
</ol>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Recall that a prime number is an integer that is greater than 1 and has no positive integer divisor other than 1 and itself. (In particular, 1 is not prime). A relation $P$ is defined on $\mathbb{Z}$ as follows

<div align="center">

For every $m$, $n$ $\in$ $\mathbb{Z}$, $m$ $P$ $n$ $\iff$ $\exists$ a prime number $p$ such that $p$ $|$ $m$ and $p$ $|$ $n$
</div>

<ol type="a">
  <li>

  Is $P$ reflexive?</li>
  <li>

  Is $P$ symmetric?</li>
  <li>

  Is $P$ transitive?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $P$ is not reflexive because when $m = 1$, then there is no prime number $p$ such that $p$ divides $m$</li>
  <li>

  $P$ is reflexive because for any integer $m$ and $n$, if $p$ is a prime number such that $p$ divides $m$ and $p$ divides $n$, then $p$ divides $n$ and $p$ divides $m$</li>
  <li> 

  Assuming $m = 12$ and $n = 15$, one can also assume that $0 = 25$. Then there is a prime number 3 that divides both $m$ and $n$ and there is a prime number 5 that divides both $n$ and $o$ and there is no prime number that divides both $m$ and $o$</li>
</ol>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $X = \{a, b, c\}$ and let $\mathcal{P}{X}$ be the power set of $X$. Define a relation $N$ on $\mathcal{P}{X}$ as follows

<div align="center">

For every $A$, $B$ $\in$ $\mathcal{P}(X)$, $A$ $N$ $B$ $\iff$ the number of elements in $A$ is not equal to the number of elements in $B$
</div>

<ol type="a">
  <li>

  Is $N$ reflexive?</li>
  <li>

  Is $N$ symmetric?</li>
  <li>

  Is $N$ transitive?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $N$ is not reflexive as by definition of $N$, this means that for every set $A$ in $\mathcal{P}{X}$, the number of elements in $A$ does not equal the number of elements in $A$. This is false</li>
  <li>

  $N$ is symmetric because if the number of elements in $B$ does not equal the number of elements in $A$, then the number of elements in $A$ does not equal the number of elements in $B$</li>
  <li> 

  $N$ is not transitive because lets say $A = \{1, 2, 3, 4, 5\}, B = \{3, 4, 5\},$ amd $C = \{3, 4, 5, 6, 7\}$. The number of elements in $A$ does not equal the number of elements in $B$; the number of elements in $B$ does not equal the number of elements $C$; however, the number of elements in $A$ equals the number of elements in $C$</li>
</ol>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $A$ be the set of all strings of 0's, 1's, and 2's that have length 4 and for which the sum of the characters in the string is less than or equal to 2. Define a relation $R$ on $A$ as follows

<div align="center">

For every $s$, $t$ $\in$ $A$, $s$ $R$ $t$ $\iff$ the sum of the characters of $S$ equals the sum of the characters of $t$
</div>

<ol type="a">
  <li>

  Is $N$ reflexive?</li>
  <li>

  Is $N$ symmetric?</li>
  <li>

  Is $N$ transitive?</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $R$ is reflexive since the sum of characters in $s$ is the same as the sum of characters in $s$</li>
  <li>

  $R$ is symmetric because if the sum of characters of $s$ equals the sum of the characters of $t$, then the sum of the characters of $t$ equals the sum of the characters of $s$</li>
  <li> 

  $R$ is transitive because if the sum of characters of $s$ equals the sum of the characters of $t$, and the sum of characters of $t$ equals the sum of the characters of $u$, then the sum of characters of $s$ equals the sum of the characters of $u$</li>
</ol>
</details>
</ul>  
</details>

## Equivalence Relations
Let $A$ be a set and $R$ a relation on $A$. $R$ is an <strong>equivalence relation</strong> if, and only if, $R$ is reflexive, symmetric, and transitive

### Equivalence Classes of an Equivalence Relation
Suppose $A$ is a set and $R$ is an equivalence relation on $A$. For each element $a$ in $A$, the <strong>equivalence class of a</strong>, denoted <strong>[a]</strong> and called the <strong>class of a</strong> for short, is the set of all elements $x$ in $A$ such that $X$ is related to $a$ by $R$

<details>
    <summary>Example problem</summary>

Let $A = \{a, b, c, d\}$ and define a relation $R$ on $A$ as follows:

<div align="center">

$R$ $=$ &#123; ($a$, $a$), ($b$, $b$), ($b$, $d$), ($c$, $c$), ($d$, $b$), ($d$, $d$) &#125;
</div>

It is a fact that $R$ is an equivalence relation on $A$. Use set-roster notation to write the equivalence classes of $R$

<ol type="a">
  <li>

  [ $a$]</li>
  <li>

  [ $b$]</li>
  <li>

  [ $c$]</li>
  <li>

  [ $d$]</li>
  <li>

  How many distinct equivalence classes does $R$ have?</li>
  <li>

  List the distinct equivalence classes of $R$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $[a] = \{a\}$</li>
  <li>

  $[b] = \{b, d\}$</li>
  <li> 

  $[c] = \{c\}$</li>
  <li>

  $[d] = \{b, d\}$</li>
  <li>There are 3 distinct equivalence classes</li>
  <li>

  The three distinct equivalence classes of $R$ are: $\{a\}, \{c\}, \{b, d\}$</li>
</ol>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $A = \{1, 2, 3, 4, ..., 18\}$ and define a relation $R$ on $A$ as follows:

<div align="center">

FOr all $x$, $y$ $\in$ $A$, $x$ $R$ $y$ $\iff$ $4$ $|$ $($ $x$ $-$ $y$ $)$
</div>

It is a fact that $R$ is an equivalence relation on $A$. Use set-roster notation to write the equivalence classes of $R$

<ol type="a">
  <li>

  [ $1$]</li>
  <li>

  [ $2$]</li>
  <li>

  [ $3$]</li>
  <li>

  [ $4$]</li>
  <li>

  [ $5$]</li>
  <li>

  How many distinct equivalence classes does $R$ have?</li>
  <li>

  List the distinct equivalence classes of $R$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

$R = \{(17, 1), (13, 1), (9, 1), (5, 1), (1, 1), (18, 2), (14, 2), (10, 2), (6, 2), (2, 2), (15, 3), (11, 3), (7, 3), (3, 3), (16, 4), (12, 4), (8, 4), (4, 4), (17, 5), (13, 5), (9, 5), (5, 5), (1, 5)\}$

<ol type="a">
  <li>

  $[1] = \{17, 13, 9, 5, 1\}$</li>
  <li>

  $[b] = \{18, 14, 10, 6, 2\}$</li>
  <li> 

  $[c] = \{15, 11, 7, 3\}$</li>
  <li>

  $[d] = \{17, 13, 9, 5, 1\}$</li>
  <li>There are 4 distinct equivalence classes</li>
  <li>

  The four distinct equivalence classes of $R$ are: $\{17, 13, 9, 5, 1\}, \{18, 14, 10, 6, 2\}, \{15, 11, 7, 3\}, \{16, 12, 8, 4\}$</li>
</ol>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $A = \{-2, -1, 0, 1, 2, 3, 4, 5, 6, 7\}$ and define a relation $R$ on $A$ as follows:

<div align="center">

FOr all $x$, $y$ $\in$ $A$, $x$ $R$ $y$ $\iff$ $3$ $|$ $($ $x$ $-$ $y$ $)$
</div>

It is a fact that $R$ is an equivalence relation on $A$. Use set-roster notation to write the equivalence classes of $R$

<ol type="a">
  <li>

  [ $0$]</li>
  <li>

  [ $1$]</li>
  <li>

  [ $2$]</li>
  <li>

  [ $3$]</li>
  <li>

  How many distinct equivalence classes does $R$ have?</li>
  <li>

  List the distinct equivalence classes of $R$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

$R = \{(6, 0), (3, 0), (0, 0), (7, 1), (4, 1), (1, 1), (-2, 1)\}$

<ol type="a">
  <li>

  $[0] = \{6, 3, 0\}$</li>
  <li>

  $[1] = \{7, 4, 1, -2\}$</li>
  <li> 

  $[2] = \{15, 11, 7, 3\}$</li>
  <li>

  $[3] = \{17, 13, 9, 5, 1\}$</li>
  <li>There are 4 distinct equivalence classes</li>
  <li>

  The four distinct equivalence classes of $R$ are: $\{17, 13, 9, 5, 1\}, \{18, 14, 10, 6, 2\}, \{15, 11, 7, 3\}, \{16, 12, 8, 4\}$</li>
</ol>
</details>
</ul>  
</details>
