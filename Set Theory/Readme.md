<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#definitions-and-the-element-method-of-proof'>Definitions and the Element Method of Proof</a>
  </li>
  <li>
    <a href='#properties-of-sets'>Properties of Sets</a>
  </li>
</ol>
</details>

## Definitions and the Element Method of Proof
Given two sets $A$ and $B$, recall that $A$ is a <strong>subset</strong> of $B$ if every element of $A$ is an element of $B$

<div align="center">

$A$ $\subseteq$ $B$ $\iff$ $\forall$ $x$ if $x$ $\in$ $A$ then $x$ $\in$ $B$
</div>

As such, $A \cancel{\subseteq} B$ when $\exists x$ : $x \in A$ but $x \notin B$

Given two sets $A$ and $B$, the two sets are <strong>equal</strong>, $A$ equals $B$, if every element of $A$ is an element of $B$ and every element of $B$ is an element of $A$

<div align="center">

$A$ $=$ $B$ $\iff$ $A$ $\subseteq$ $B$ and $B$ $\subseteq$ $A$
</div>

If $A$ is a subset of $B$, but $A \cancel{=} B$, $A$ is called a <strong>proper subset</strong> of $B$, which can also be written as $A \subsetneq B$. This occurs when $A \subseteq B$, but at least one element of $B$ is not also in $A$

<details>
    <summary>Example problem</summary>

Let the universal set be $\mathbb{R}$, the set of all real numbers, and let $A =$ { $x \in \mathbb{R} | -3 \leq x \leq 0$ } $, B =$ { $x \in \mathbb{R} | -1 < x < 2$ } , and $C =$ { $x \in \mathbb{R} | 6 < x \leq 8$ }. Find each of the following:

<ol type="a">
  <li>

  $A \cup B$</li>
  <li>

  $A \cap B$</li>
  <li>

  $A$<sup>c</sup></li>
  <li>

  $A \cup C$</li>
  <li>

  $A \cap C$</li>
  <li>

  $B$<sup>c</sup></li>
  <li>

  $A$<sup>c</sup> $\cap B$<sup>c</sup></li>
  <li>

  $A$<sup>c</sup> $\cup B$<sup>c</sup></li>
  <li>

  $(A \cap B)$<sup>c</sup></li>
  <li>

  $(A \cup B)$<sup>c</sup></li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $A \cup B$ = { $x \in \mathbb{R} | -3 \leq x < 2$ }</li>
  <li>

  $A \cap B$ = { $x \in \mathbb{R} | -1 < x \leq 0$ }</li>
  <li>

  $A$<sup>c</sup> = { $x \in \mathbb{R} | x < 3$ or $x > 0$ }</li>
  <li>

  $A \cup C$ = { $x \in \mathbb{R} | -3 \leq x \leq 0$ or $6 < x \leq 8$ }</li>
  <li>

  $A \cap C$ = $\emptyset$</li>
  <li>

  $B$<sup>c</sup> = { $x \in \mathbb{R} | x \geq 2$ or $x \leq -1$ }</li>
  <li>

  $A$<sup>c</sup> $\cap B$<sup>c</sup> = { $x \in \mathbb{R} | x < -3$ or $x \geq 2$ }</li>
  <li>

  $A$<sup>c</sup> $\cup B$<sup>c</sup> = { $x \in \mathbb{R} | -1 \geq x$ or $x > 0$ }</li>
  <li>

  $(A \cap B)$<sup>c</sup> { $x \in \mathbb{R} | x \leq 1$ or $x > 0$ }</li>
  <li>

  $(A \cup B)$<sup>c</sup> { $x \in \mathbb{R} | -3 > x$ or $x \geq 2$ }</li>
</ol>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $S$ be the set of all strings of 0's and 1's of length 4, and let $A$ and $B$ be the following subsets of $S$

<div align="center">

$A =$ { $1000, 1101, 0101, 1100$ } and $B =$ { $ 0110, 1001, 1100, 0011$ }
</div> 

Find each of the following:

<ol type="a">
  <li>

  $A \cap B$</li>
  <li>

  $A \cup B$</li>
  <li>

  $A - B$</li>
  <li>

  $B - A$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $A \cap B =$ { $1100$ }</li>
  <li>

  $A \cup B =$ { $1000, 1101, 0101, 1100, 0110, 1001, 0011$ }</li>
  <li>

  $A - B =$ { $1000 1101, 0101$ }</li>
  <li>

  $B - A =$ { $0110, 1001, 0011$ }</li>
</ol>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $A =$ { $a, b, c$ }, $B =$ { $b, c, d$ }, $C =$ { $b, c, e$ }

<ol type="a">
  <li>

  Find $A \cup (B \cap C), (A \cup B) \cap C,$ and $(A \cup B) \cap (A \cup C)$</li>
  <li>

  Find $A \cap (B \cup C), (A \cap B) \cup C,$ and $(A \cap B) \cup (A \cap C)$</li>
  <li>

  Find $(A - B) - C$ and $A - (B - C)$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $A \cup (B \cap C) = A \cup$ { $b, c$ } = { $a, b, c$ }<br />
  $A \cup (B \cap C) =$ { $a, b, c, d$ } $\cap C =$ { $b, c$ }<br />
  $(A \cup B) \cap (A \cup C) =$ { $a, b, c, d$ } $ \cup$ { $a, b, c, e$ } = { $a, b, c$ }</li>
  <li>

  $A \cap (B \cup C) = A \cap$ { $b, c, d, e$ } = { $b, c$ }<br />
  $(A \cap B) \cup C =$ { $b, c$ } $\cup C =$ { $b, c, e$ }<br />
  $(A \cap B) \cup (A \cap C) =$ { $b, c$ } $\cup$ { $b, c$ } = { $b, c$ }</li>
  <li>

  $(A - B) - C =$ { $a$ } - { $b, c, e$ } = { $a$ }<br />
  $A - (B - C) =$ { $a, b, c$ } - { $d$ } = { $a, b, c$ }</li>
</ol>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $B$<sub>i</sub> = { $x \in \mathbb{R} | 0 \leq x \leq i$ } for each integer $i = 1, 2, 3, 4$

<ol type="a">
  <li>

  Find $B$<sub>1</sub> $\cup B$<sub>2</sub> $\cup B$<sub>3</sub> $\cup B$<sub>4</sub></li>
  <li>

  Find $B$<sub>1</sub> $\cap B$<sub>2</sub> $\cap B$<sub>3</sub> $\cap B$<sub>4</sub></li>
  <li>

  Find $(A - B) - C$ and $A - (B - C)$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $A \cup (B \cap C) = A \cup$ { $b, c$ } = { $a, b, c$ }<br />
  $A \cup (B \cap C) =$ { $a, b, c, d$ } $\cap C = $ { $b, c$}<br />
  $(A \cup B) \cap (A \cup C) =$ { $a, b, c, d$ } $\cup $ { $a, b, c, e$ } = { $a, b, c$ }</li>
  <li>

  $A \cap (B \cup C) = A \cap$ { $b, c, d, e$ } = { $b, c$ }<br />
  $(A \cap B) \cup C =$ { $b, c$ } $\cup C =$ { $b, c, e$ }<br />
  $(A \cap B) \cup (A \cap C) =$ { $b, c$ } $\cup$ { $b, c$ } = { $b, c$ }</li>
  <li>

  $(A - B) - C =$ { $a$ } - { $b, c, e$ } = { $a$ }<br />
  $A - (B - C) =$ { $a, b, c$ } - { $d$ } = { $a, b, c$ }</li>
</ol>
</details>
</ul>  
</details>

### Venn Diagrams
<strong>Venn diagrams</strong> are used to present relation among sets

If $A \subseteq B$, then
<img width=500px, height=200px, src="Images/Diagrams/Diagram 1.png" alt="Diagram 1">

If $A \cancel{\subseteq} B$, then
<img width=500px, height=200px, src="Images/Diagrams/Diagram 2.png" alt="Diagram 2">

<details>
    <summary>Example problem</summary>

$U =$ { $a, b, c, d, e, f, g, h, i, j$ }<br />
$C =$ { $d, e, g, i$ }<br />
$Y =$ { $b, c, d, g, h, i$ }<br />
$Z =$ { $a, b, e, h, i$ }<br />

where $U$ is the universal set containing $X$, $Y$, and $Z$<br />

Determine the elements of

<div align="center">

$($ $X$ $-$ $($ $Z$ $\land$ $Y$ $)$ $)$<sup>C</sup>
</div>
<ul>  
  <details>
    <summary>Solution</summary>

<img width=500px, height=200px, src="Images/Example Problems/Diagram 3A.png" alt="Diagram 3A">
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Select two of the following sets that are disjoin:<br />
$A \vee B$<sup>C</sup><br />
$A$<sup>C</sup> $\vee B$<br />
$A \land B$<sup>C</sup><br />
$A$
</div>
<ul>  
  <details>
    <summary>Solution</summary>

<img width=500px, height=200px, src="Images/Example Problems/Diagram 4A.png" alt="Diagram 4A">
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Use a Venn diagram which regions correspond to the sets $C \land (B \vee A)$ and $B \vee (C \land A)$
</div>
<ul>  
  <details>
    <summary>Solution</summary>

<img width=500px, height=200px, src="Images/Example Problems/Diagram 5A.png" alt="Diagram 5A">
</details>
</ul>  
</details>

### Set Operations
The set of interest is called the <strong>universal set</strong> or <strong>universe</strong> often set as $U$

The <strong>union</strong> of $A$ and $B$ is the set formed by taking members belonging to $A$, $B$, or both, to make another set:

<div align="center">

$A$ $\cup$ $B$
</div>

The <strong>intersection</strong> of $A$ and $B$ is the set formed by taking members common to both $A$ and $B$ to make another set:

<div align="center">

$A$ $\cap$ $B$
</div>

The <strong>difference</strong> or <strong>relative complement</strong> of $A$ and $B$ is the set formed by taking members belonging to $A$, but not $B$, to make another set:

<div align="center">

$A$ $-$ $B$ = { $x$ : $x$ $\in$ $A$ but $x$ $\notin$ $B$ }
</div>

The <strong>complement</strong> of $A$, denoted $A$<sup>c</sup>, is the set of all elements in $U$ that are not in $A$

<img src="Images/Diagrams/Diagram 3.png" alt="Diagram 3">

<details>
    <summary>Example problem</summary>

Let $U =$ { $1, 2, 3, 4, 5, 6, 7$ } be the universal set containing $A = $ { $1, 3, 5, 7$ } and $B =$ { $4, 5, 6, 7$ }. Then find

<ol type="a">
  <li>

  $A \cup B$</li>
  <li>

  $A \cap B$</li>
  <li>

  $A - B$</li>
  <li>

  $B - A$</li>
  <li>

  $A$<sup>c</sup></li>
  <li>

  $B$<sup>c</sup></li>
  <li>

  $(A \cup B)$<sup>c</sup></li>
  <li>

  $(A \cap B)$<sup>c</sup></li>
  <li>

  $A$<sup>c</sup> $\cap B$<sup>c</sup></li>
  <li>

  $A$<sup>c</sup> $\cup B$<sup>c</sup></li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<img src="Images/Example Problems/Problem 1A.png" alt="Problem 1A">
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $A =$ { $1, 3, 5, 7, 9$ }, $B =$ {$3, 6, 9$ }, and $C =$ { $2, 4, 6, 8$ }. Find each of the following

<ol type="a">
  <li>

  $A \cup B$</li>
  <li>

  $A \cap B$</li>
  <li>

  $A \cup C$</li>
  <li>

  $A \cap C$</li>
  <li>

  $A - B$</li>
  <li>

  $B - A$</li>
  <li>

  $B \cup C$</li>
  <li>

  $B \cap C$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<img src="Images/Example Problems/Problem 2A.png" alt="Problem 2A">
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Select all statements below which are generally true for sets $A$, $B$, and $C$:<br />
<ul>
  <li>
  
  If $A \subset B$ and $B \land C = \empty$ then $C \land A = \empty$</li>
  <li>

  $(C \vee A)$<sup>C</sup> $- B = (A \vee B \vee C)<sup>C</sup></li>
  <li>

  If $A$<sup>C</sup> $\subset B$<sup>C</sup> then $B \subset A$</li>
  <li>  

  <li>

  $A - C = (A - B) \vee (B - C)$</li>
<ul>  
  <details>
    <summary>Solution</summary>

<img src="Images/Example Problems/Problem 6A.png" alt="Problem 6A">
</details>
</ul>  
</details>

### Partitions of Sets
Two sets $A$ and $B$ are said to be <strong>disjoint</strong> if $A \cap B = \emptyset$ and if and only if, they have no elements in common

<details>
    <summary>Example problem</summary>

Express the complement of (-3, 9) $\land$ [-5, 4]
<ul>  
  <details>
    <summary>Solution</summary>

<img src="Images/Example Problems/Problem 7A.png" alt="Problem 7A">
</details>
</ul>  
</details>

Sets $A$<sub>1</sub>, $A$<sub>2</sub>, and $A$<sub>3</sub> are <strong>mutually disjoint</strong> if, and only if, no two sets $A$<sub>i</sub> and $A$<sub>j</sub> with distinct subscripts have any elements in common

<details>
    <summary>Example problem</summary>

Let $B$<sub>i</sub> = { $x \in \mathbb{R} | 0 \leq x \leq i$ } for each integer $i = 1, 2, 3, 4$

<ol type="a">
  <li>

  Find $B$<sub>1</sub> $ \cup B$<sub>2</sub> $ \cup B$<sub>3</sub> $\cup B$<sub>4</sub></li>
  <li>

  Find $B$<sub>1</sub> $\cap B$<sub>2</sub> $\cap B$<sub>3</sub> $\cap B$<sub>4</sub></li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $B$<sub>1</sub> $ \cup B$<sub>2</sub> $ \cup B$<sub>3</sub> $\cup B$<sub>4</sub> $ = [0, 4]$</li>
  <li>

  $B$<sub>1</sub> $\cap B$<sub>2</sub> $\cap B$<sub>3</sub> $\cap B$<sub>4</sub> $ = [0, 1]$</li>
</ol>
None of the sets are disjoint because each set contains the real numbers ranging from [0, 1]
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $V$<sub>i</sub> = { $x \in \mathbb{R} | -1 / i \leq x \leq 1/i$ } = [ $-1/i, 1/i$ ] for each positive integer $i$. Find each of the following:

<ol type="a">
  <li>

  $\bigcup_{i=1}^{4} V_i =$</li>
  <li>

  $\bigcap_{i=1}^{4} V_i =$</li>
  <li>

  Are $V$<sub>1</sub>, $V$<sub>2</sub>, $V$<sub>3</sub>, ... mutually disjoint?</li>
  <li>

  $\bigcup_{i=1}^{n} V_i = \\$</li>
  <li>

  $\bigcap_{i=1}^{n} V_i = \\$</li>
  <li>

  $\bigcup_{i=1}^{\infty} V_i = \\$</li>
  <li>

  $\bigcap_{i=1}^{\infty} V_i =$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $\bigcup_{i=1}^{4} V_i = [-1, 1]$</li>
  <li>

  $\bigcap_{i=1}^{4} V_i = [-1/4, 1/4]$</li>
  <li>The sets are not mutually disjoint because no two of the sets are disjoint</li>
  <li>

  $\bigcup_{i=1}^{n} V_i = [-1, 1]$</li>
  <li>

  $\bigcap_{i=1}^{n} V_i = [-1/n, 1/n]$</li>
  <li>

  $\bigcup_{i=1}^{\infty} V_i = [-1, 1]$</li>
  <li>

  $\bigcap_{i=1}^{\infty} V_i = (0)$</li>
</ol>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Let $V$<sub>i</sub> = { $x \in \mathbb{R} | 1 \leq x \leq 1 + 1/i$ } = [ $1, 1 + 1/i$ ] for each positive integer $i$. Find each of the following:

<ol type="a">
  <li>

  $\bigcup_{i=1}^{7} R_i =$</li>
  <li>

  $\bigcap_{i=1}^{4} R_i =$</li>
  <li>

  Are $R$<sub>1</sub>, $R$<sub>2</sub>, $R$<sub>3</sub>, ... mutually disjoint?</li>
  <li>

  $\bigcup_{i=1}^{n} R_i = \\$</li>
  <li>

  $\bigcap_{i=1}^{n} R_i = \\$</li>
  <li>

  $\bigcup_{i=1}^{\infty} R_i = \\$</li>
  <li>

  $\bigcap_{i=1}^{\infty} R_i =$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>

  $\bigcup_{i=1}^{4} V_i = [-1, 1] = [1, 2]$</li>
  <li>

  $\bigcap_{i=1}^{4} V_i = [-1/4, 1/4] = [1, 8/7]$</li>
  <li>The sets are not mutually disjoint because no two of the sets are disjoint</li>
  <li>

  $\bigcup_{i=1}^{n} V_i = [1, 2]$</li>
  <li>

  $\bigcap_{i=1}^{n} V_i = [1, 1 + 1/n]$</li>
  <li>

  $\bigcup_{i=1}^{\infty} V_i = [-1, 2]$</li>
  <li>

  $\bigcap_{i=1}^{\infty} V_i = [1, 1]$</li>
</ol>
</details>
</ul>  
</details>

A finite or infinite collection of nonempty sets is a <strong>partition</strong> of a set $A$, if, and only if,
<ol>
  <li>

  $A$ is the union of all the $A$<sub>i</sub></li>
  <li>
  
  The sets $A$<sub>1</sub>, $A$<sub>2</sub>, $A$<sub>3</sub>, ... are mutually disjoint</li>
</ol>  

<details>
    <summary>Example problem</summary>
<ol type="a">
  <li>

  Is {{ $a, d, e$ }, { $b, c$ }, { $d, f$ }} a partition of { $a, b, c, d, e, f$ }</li>
  <li>

  Is {{ $w, x, v$ }, { $u y q$ }, { $p, z$ }} a partition of { $p, q, u, v, w, x, y, z$ }</li>
  <li>

  Is {{ $5, 4$ }, { $7, 2$ }, { $1, 3, 4$ }, { $6, 8$ }} a partition of {{ $1, 2, 3, 4, 5, 6, 7, 8$ }}</li>
  <li>
  
  Is {{ $3, 7, 8$ }, { $2, 9$ }, { $1, 4, 5$ }} a partition of { $1, 2, 3, 4, 5, 6, 7, 8, 9$ }</li>
  <li>

  is {{ $1, 5$ }, { $4, 7$ }, { $2, 8, 6, 3$ }} a partition of { $1, 2, 3, 4, 5, 6, 7, 8$ }</li>
  <li>

  $\bigcup_{i=1}^{\infty} R_i = \\$</li>
  <li>

  $\bigcap_{i=1}^{\infty} R_i =$</li>
</ol>
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>It is not a partition because the sets are not mutually disjoint</li>
  <li>Yes it is partition</li>
  <li>The sets are not mutually disjoint because no two of the sets are disjoint</li>
  <li>It is not a partition because the sets are not mutually disjoint</li>
  <li>It is not a partition because the element 6 is not a member of any of the other sets</li>
  <li>Yes</li>
</ol>
</details>
</ul>  
</details>

### Power Sets
The <strong>power set</strong> of a set $S$ is the set of all possible subsets of $S$, including the empty set and $S$ itself

Given the set $A$, the power set of $A$ is denoted by $\mathcal{P}(A)$

<details>
    <summary>Example problem</summary>

Let $X = $ { $a, b, c$ }. Define a relation $J$ on $\mathcal{P}(X)$ as follows:<br /><br />
For all sets $A$ and $B$ in $\mathcal{P}(X)$,<br />$A J B \iff A \cap B \cancel{=} \emptyset$

<ol type="a">
  <li>
  
  Is { $a$ } $J$ { $c$ }</li>
  <li>
  
  Is { $a, b$ } $J$ { $b, c$ }</li>
  <li>
  
  Is { $a, b$ } $J$ { $a, b, c$ }</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>No</li>
  <li>Yes</li>
  <li>Yes</li> 
</ol>
</details>
</ul>  
</details>

## Properties of Sets
<body>
    <table>
        <tr>
            <th>Law</th>
            <th>Expression</th>
        </tr>
        <tr>
            <td>Commutative Laws</td>
            <td>

$(a) A \cup B = B \cup A$<br />
$(b) A \cap B = B \cap A$
            </td>
        </tr>
        <tr>
            <td>Associative Laws</td>
            <td>
                $(a) (A \cup B) \cup C = A \cup (B \cup C)$ <br>
                $(b) (A \cap B) \cap C = A \cap (B \cap C)$
            </td>
        </tr>
        <tr>
            <td>Distributive Laws</td>
            <td>
                $(a) A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$<br>
                $(b) A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$
            </td>
        </tr>
        <tr>
            <td>Identity Laws</td>
            <td>
                $(a) A \cup \emptyset = A$<br>
                $(b) A \cap U = A$
            </td>
        </tr>
        <tr>
            <td>Complement Laws</td>
            <td>
                $(a) A \cup A^c = U$<br>
                $(b) A \cap A^c = \emptyset$
            </td>
        </tr>
        <tr>
            <td>Double Complement Law</td>
            <td>$(A^c)^c = A$</td>
        </tr>
        <tr>
            <td>Idempotent Laws</td>
            <td>
                $(a) A \cup A = A$<br>
                $(b) A \cap A = A$
            </td>
        </tr>
        <tr>
            <td>Universal Bound Laws</td>
            <td>
                $(a) A \cup U = U$<br>
                $(b) A \cap \emptyset = \emptyset$
            </td>
        </tr>
        <tr>
            <td>De Morgan’s Laws</td>
            <td>
                $(a) (A \cup B)^c = A^c \cap B^c$ <br>
                $(b) (A \cap B)^c = A^c \cup B^c$
            </td>
        </tr>
        <tr>
            <td>Absorption Laws</td>
            <td>
                $(a) A \cup (A \cap B) = A$<br>
                $(b) A \cap (A \cup B) = A$
            </td>
        </tr>
        <tr>
            <td>Complements of $U$ and $\emptyset$</td>
            <td>
                $(a) U^c = \emptyset$<br>
                $(b) \emptyset^c = U$
            </td>
        </tr>
        <tr>
            <td>Set Difference Law</td>
            <td>$A - B = A \cap B^c$</td>
        </tr>
        <tr>
            <td>Inclusion of Intersection</td>
            <td>
                $(a) A \cap B \subseteq A$<br>
                $(b) A \cap B \subseteq B$
            </td>
        </tr>
        <tr>
            <td>Inclusion in Union</td>
            <td>
                $(a) A \subseteq A \cup B$<br>
                $(b) B \subseteq A \cup B$
            </td>
        </tr>
        <tr>
            <td>Transitive Property of Subsets</td>
            <td>If $A \subseteq B$ and $B \subseteq C$, then $A \subseteq C$.</td>
        </tr>
    </table>
</body>

<details>
    <summary>Example problem</summary>

Prove that $(A - B) \cap (C - B) \subseteq (A \cap C) - B$
<ul>  
  <details>
    <summary>Solution</summary>

$x \in A - B$ and $x \in C - B \quad$ By definition of intersection<br />
$(A \cap B^c) \cap (C \cap B^c) \quad$ By Set Difference Law<br />
Thus, $x \in A \cap C$ and $x \notin B$ by 
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Prove that $(A \cap C) - B \subseteq (A - B) \cap (C - B)$
<ul>  
  <details>
    <summary>Solution</summary>

$x \in A \cap C$ and $x \notin B$ By definition of set difference<br />
Thus, bu definition of intersection, $x \in A$ and $x \in C$, and, in addition, $x \notin B$<br />
Hence, both $x \in A$ and $x \in B$ and also $x \in C$ and $x \notin B$<br />
So by definition of set difference, $x \in A - B$ and $x \in C - B$<br />
By definition of intersection, $x \in (A - B) \cap (C - B) \quad$<br />
Hence, $(A \cap C) - B \subseteq (A - B) \cap (C - B) \quad$ by definition of subset</details>
</ul>  
</details>
