<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#logic-form-and-logical-equivalence'>Logic Form and Logical Equivalence</a>
  </li>
  <li>
    <a href='#conditional-logic'>Conditional Logic</a>
  </li>
  <li>
    <a href='#valid-and-invalid-arguments'>Valid and Invalid Arguments</a>
  </li>
</ol>
</details>

## Logic Form and Logical Equivalence
### Statements
A <strong>statement</strong> (or <strong>proposition</strong>) is a sentence that is true or false, but not both

<ul>
  <li>Some examples of statements are: "two plus two equals four" and "two plus two equals five" are both statements. This is because the statements are definitively true or false. The first statement is true and the second statement is false</li>
  <li>On the other hand, "x + y > 0" is not a statement because this expression without further context cannot be evaluated to true or false without knowing what the values of x and y are. For some values of x and y can make this expression true, for other values, the expression can be false; therefore, this expression is not a statement</li>
</ul>  

The relation between equals and equivalence is that equals refer to sameness in value. Equivalence, however, denotes things that are not identical but have a similar or equal effect or value

### Compound Statements
The <strong>negation of 
$p$</strong> is given by the following statement: $\neg p$. This $\neg$ symbol denotes $not$, meaning that $\neg p$ means not $p$

The <strong>
conjunction of $p$ and $q$</strong> is given by the following statement: $p \land q$. This $\land$ symbol is read as $p$ and $q$

The <strong>disjunction of 
$p$ and $q$</strong> is given by the following statement: $p \vee q$. This $\vee$ symbol is read as $p$ or $q$.

In more complex statements, such as compound statements, there is an <strong>order of operations</strong> that specifies which parts of an expression are evaluated first

<ol>
  <li>

$\neg$ has the highest precedence, meaning that $\neg$ is performed first</li>

  <li>
  
The statements $\land$ and $\vee$ are coequal in order of precedence. For instance, an expression such as $p \land q \vee r$ is considered ambiguous as an expression like this must be written like $(p \land q) \vee r$ or $p \land (q \vee r)$ to have meaning</li>
</ol>

<div align="center">

$p$ but $q$ $\quad$ means $\quad$ $p$ and $q$<br />
neither $p$ nor $q$ $\quad$ means $\quad$ $\neg$ $p$ and $\neg$ $q$
</div>

<details>
    <summary>Example problem</summary>
Write each of the following sentences symbolically, letting $h$ = "It is hot" and $s$ = "It is sunny".<br />
a) It is not hot but it is sunny<br />
b) It is neither hot nor sunny
<ul>  
  <details>
    <summary>Solution</summary>

a) $\neg h \land s$<br />
b) $\neg h \land \neg s$

</details>
</ul>  
</details>  

The notation for inequalities involves $and$ and $or$ statements. For instance, if $x$, $a$, and $b$ are particular real numbers, then

<div align="center">

$x$ $\leq$ $a$ $\quad$ means $\quad$ $x$ $<$ $a$ or $x$ $=$ $a$<br />
$a$ $\leq$ $x$ $\leq$ $b$ $\quad$ means $\quad$ $a$ $\leq$ $x$ and $x$ $\leq$ $b$
</div>

<details>
    <summary>Example problem</summary>

Suppose $x$ is a particular real number. Let $p$, $q$, and $r$ symbolize 0 < $x$, $x$ < 3, and $x$ = 3, respectively. Write the following inequalities symbolically:<br />
a) $x \leq$ 3<br />
b) 0 < $x$ < 3<br />
c)0 < $x \leq$ 3
<ul>  
  <details>
    <summary>Solution</summary>

a) $q \vee r$<br />
b) $p \land q$<br />
c) $p \land (q \vee r)$

</details>
</ul>  
</details>  

### Truth Values
As in the examples above, compound sentences can be made out of component statements using $not$, $and$, and $or$. If those sentences are to be statements, they must have <strong>truth values</strong> that are either true or false

If $p$ is a statement, the <strong>negation</strong> of $p$ is "not $p$". It has the opposite truth value from $p$. If $p$ is true, $\neg p$ is false; otherwise, if $p$ is false, $\neg p$ is true

<h3 align="center">Truth Table for $\neg p$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$\neg p$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
  </tr>
</table>

If $p$ and $q$ are statement variables, the <strong>conjunction</strong> of $p$ and $q$ is denoted as $p \land q$. It is true when both $p$ and $q$ are true; otherwise, if $p$, $q$, or $p$ and $q$ are false, then $p \land q$ is false

<h3 align="center">Truth Table for $p \land q$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$p \land q$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
</table>

If $p$ and $q$ are statement variables, the <strong>disjunction</strong> of $p$ and $q$ is denoted as $p \vee q$. It is true when either $p$ is true, $q$ is true, or both $p$ and $q$ are true; it is only false when both $p$ and $q$ are false

<h3 align="center">Truth Table for $p \lor q$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$p \lor q$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
</table>

<details>
    <summary>Example problem</summary>

Construct a truth table for the statement form $(p \land q) \vee \neg r$
<ul>  
  <details>
    <summary>Solution</summary>

<h3 align="center">Truth Table for $(p \land q) \vee \neg r$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$r$</th>
    <th>$p \land q$</th>
    <th>$\neg r$</th>
    <th>$(p \land q) \vee \neg r$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
  </tr>
</table>
</details>
</ul>  
</details>  

### Logical Equivalence
Two statement forms are <strong>logically equivalent</strong> if and only if they have identical truth values for each possible arrangement of values for their statement variables. The logical equivalence of statement forms $P$ and $Q$ is denoted by writing $P \equiv Q$

To test whether two statement forms $P$ and $Q$ are logically equivalent
<ol>
  <li>

Construct a truth table with one column for the truth values of $P$ and another column for the truth values of $Q$</li>
  <li>

Check each combination of truth values of the statement variables to see whether the truth value of $P$ is the same as the truth value of $Q$
    <ol type="a">
      <li>If in each row of the truth table the value of $P$ is the same as the truth value of $Q$, the $P$ and $Q$ are logically equivalent</li>
      <li>If in some row $P$ has a different truth value from $Q$, then $P$ and $Q$ are not logically equivalent</li>
    </ol>
  </li>
</ol>      

Double negative property:

$$
\neg(\neg p) \equiv p
$$

<details>
    <summary>Example problem</summary>

Construct a truth table to show that the negation of the negation of a statement is logically equivalent to the statement 
<ul>  
  <details>
    <summary>Solution</summary>

<h3 align="center">Truth Table for $\neg(\neg p)$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$\neg p$</th>
    <th>$\neg(\neg p)$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>F</td>
  </tr>
</table>
</details>
</ul>  
</details>  

<details>
    <summary>Example problem</summary>

Show that the statement forms $\neg(p \land q)$ and $\neg p \land \neg q$ are not logically equivalent
<ul>  
  <details>
    <summary>Solution</summary>

<h3 align="center">Truth Tables for $\neg(p \land q)$ and $\neg p \land \neg q$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$\neg p$</th>
    <th>$\neg q$</th>
    <th>$p \land q$</th>
    <th>$\neg(p \land q)$</th>
    <th>$\neg p \land \neg q$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
  </tr>
</table>
</details>
</ul>  
</details>  

### De Morgan's Laws
The negation of the conjunction of two statements is logically equivalent to the disjunction of their negations:

$$
\neg(p \land q) \equiv \neg p \vee \neg q
$$

The negation of the disjunction of two statements is logically equivalent to the conjunction of their negations:

$$
\neg(p \vee q) \equiv \neg p \land \neg q
$$

<details>
    <summary>Example problem</summary>

Write negations for each of the following statements:<br />
<ol type="a">
  <li>John is 6 feet tall and he weights at least 200 pounds.</li>
  <li>The bus was late or Tom's watch was slow.</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>John is not 6 feet tall or he does not weigh at least 200 pounds.</li>
  <li>The bus was not late and Tom's watch was not slow.</li>
</ol>  
</details>
</ul>  
</details>  

<details>
    <summary>Example problem</summary>

Use De Morgan's law to write the negation of -1 $<$ x $\leq$ 4
<ul>  
  <details>
    <summary>Solution</summary>

-1 $< x$ and $x \leq$ 4

$\neg$(-1 $< x$)$\quad$=$\quad$-1 $\geq x$

$\neg$($x \leq$ 4)$\quad$=$\quad x >$ 4

$\neg$(-1 $< x \leq$ 4)$\quad$=$\quad$-1 $\geq x \vee x >$ 4

</details>
</ul>  
</details>

### Tautologies and Contradictions

A <strong>tautology</strong> is a statement that is always true regardless of the truth values of its components. A statement whose form is a tautology is a <strong>tautological statement</strong>

A <strong>contradiction</strong> is a statement form that is always false regardless of the truth values of its components. A statement whose form is a contradiction is a <strong>contradictory statement</strong>

<details>
    <summary>Example problem</summary>

Show that the statement form $p \vee \neg p$ is a tautology and that the statement form $p \land \neg p$ is a contradiction
<ul>  
  <details>
    <summary>Solution</summary>

<h3 align="center">Truth Tables for $p \vee \neg p$ and $p \land \neg p$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$\neg p$</th>
    <th>$p \vee \neg p$</th>
    <th>$p \land \neg p$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
  </tr>
</table>
</details>
</ul>  
</details>

<body>
    <h3 align="center">Table of Logical Equivalences</h3>
    <div align="center">
        <table border="1" cellpadding="10" cellspacing="0">
            <thead>
                <tr>
                    <th>Law</th>
                    <th>Logical Equivalence</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Commutative Laws</td>
                    <td>$p \land q \equiv q \land p$, $\quad p \lor q \equiv q \lor p$</td>
                </tr>
                <tr>
                    <td>Associative Laws</td>
                    <td>$(p \land q) \land r \equiv p \land (q \land r)$, $\quad (p \lor q) \lor r \equiv p \lor (q \lor r)$</td>
                </tr>
                <tr>
                    <td>Distributive Laws</td>
                    <td>$p \land (q \lor r) \equiv (p \land q) \lor (p \land r)$, $\quad p \lor (q \land r) \equiv (p \lor q) \land (p \lor r)$</td>
                </tr>
                <tr>
                    <td>Identity Laws</td>
                    <td>$p \land t \equiv p$, $\quad p \lor c \equiv p$</td>
                </tr>
                <tr>
                    <td>Negation Laws</td>
                    <td>$p \lor \neg p \equiv t$, $\quad p \land \neg p \equiv c$</td>
                </tr>
                <tr>
                    <td>Double Negative Law</td>
                    <td>$\neg (\neg p) \equiv p$</td>
                </tr>
                <tr>
                    <td>Idempotent Laws</td>
                    <td>$p \land p \equiv p$, $\quad p \lor p \equiv p$</td>
                </tr>
                <tr>
                    <td>Universal Bound Laws</td>
                    <td>$p \lor t \equiv t$, $\quad p \land c \equiv c$</td>
                </tr>
                <tr>
                    <td>De Morgan’s Laws</td>
                    <td>$\neg (p \land q) \equiv \neg p \lor \neg q$, $\quad \neg (p \lor q) \equiv \neg p \land \neg q$</td>
                </tr>
                <tr>
                    <td>Absorption Laws</td>
                    <td>$p \lor (p \land q) \equiv p$, $\quad p \land (p \lor q) \equiv p$</td>
                </tr>
                <tr>
                    <td>Negations of $t$ and $c$</td>
                    <td>$\neg t \equiv c$, $\quad \neg c \equiv t$</td>
                </tr>
            </tbody>
        </table>
    </div>
</body>

<details>
    <summary>Example problem</summary>

Verify the following logical equivalence: $\neg(\neg p \land q) \land (p \vee q) \equiv p$
<ul>  
  <details>
    <summary>Solution</summary>

$\equiv p \vee \neg q \land (p \vee q) \quad$ De Morgan's Law

$\equiv (p \vee \neg q) \land (p \vee q) \quad$ Distributive Law

$\equiv p \vee (\neg q \vee q) \quad$ Distributive Law

$\equiv p \vee 1 \quad$ Universal Bound's Law

$\equiv p$
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Verify the following logical equivalence: $(p \land \neg q) \vee p \equiv p$
<ul>  
  <details>
    <summary>Solution</summary>

$\equiv p \quad$ Absorption Law
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Verify the following logical equivalence: $\neg((\neg p \land q) \vee (\neg p \land \neg q)) \vee (p \land q) \equiv p$
<ul>  
  <details>
    <summary>Solution</summary>

$\equiv \neg(\neg p \land (q \vee \neg q)) \vee (p \land q) \quad$ Distributive Law

$\equiv \neg(\neg p \land t) \vee (p \land q) \quad$ Negation Law

$\equiv \neg(\neg p) \vee (p \land q) \quad$ Identity Law

$\equiv p \vee (p \land q) \quad$ Double Negative Law

$\equiv p \quad$ Absorption Law
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Verify the following logical equivalence: $(p \land (\neg(\neg p \vee q))) \vee (p \land q) \equiv p$
<ul>  
  <details>
    <summary>Solution</summary>

$\equiv (p \land (p \land \neg q)) \vee (p \land q) \quad$ De Morgan's Law

$\equiv (\neg q \land (p \land p)) \vee (p \land q) \quad$ Associative Law

$\equiv (\neg q \land p) \vee (p \land q) \quad$ Idempotent Law

$\equiv p \land (\neg q \vee q) \quad$ Distributive Law

$\equiv p \land t \quad$ Negation Law

$\equiv p \quad$ Identity Law
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Use algebra to verify that $p \vee q \rightarrow r \equiv \neg(p \vee q) \vee r$
<ul>  
  <details>
    <summary>Solution</summary>

$\equiv (p \vee q) \rightarrow r$

$\equiv \neg(p \vee q) \vee r$
</details>
</ul>  
</details>

### Exclusive Or
The <strong>exclusive or</strong> $p \oplus q$ is true whenever exactly one of $p$ and $q$ are true, but not both or neither. It is an easy exercise to confirm that

<div align="center">

$p$ $\oplus$ $q$ $\equiv$ $($ $p$ $\land$ $\neg$ $q$ $)$ $\vee$ $($ $\neg$ $p$ $\land$ $q$ $)$
</div>

## Conditional Statements
If $p$ and $q$ are statement variables, the <strong>conditional</strong> of $q$ by $p$ is "if $p$ than $q$" and is denoted $p \rightarrow q$. It is false when $p$ is true and $q$ is false; otherwise, it is true. $p$ is called the <strong>hypotheses</strong> (or <strong>antecedent</strong>) of the conditional and $q$ the <strong>conclusion</strong> (or <strong>consequent</strong>)

A conditional statement that is true by virtue of the fact that its hypothesis is false is called <strong>vacuously true</strong> or <strong>true by default</strong>. This is because the if-then statement will always be true when the hypothesis is true, regardless of what the conclusion is

In expressions that include $\rightarrow$ as well as other logical operators such as $\land$, $\vee$, and $\neg$, the <strong>order of operations</strong> is that $\rightarrow$ is performed last

<details>
    <summary>Example problem</summary>

Construct a truth table for the statement form $p \vee \neg q \rightarrow \neg p$
<ul>  
  <details>
    <summary>Solution</summary>

<h3 align="center">Truth Table for $p \lor q$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$\neg q$</th>
    <th>$p \vee \neg q$</th>
    <th>$\neg p$</th>
    <th>$p \vee \neg q \rightarrow p$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
</table>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Use truth tables to show the logical equivalence of the statement forms $p \vee q \rightarrow r$ and $(p \rightarrow r) \land (q \rightarrow r)$. Annotate the table with a sentence of explanation
<ul>  
  <details>
    <summary>Solution</summary>

<h3 align="center">Truth Table for $p \lor q$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$r$</th>
    <th>$p \vee q$</th>
    <th>$p \rightarrow r$</th>
    <th>$q \rightarrow r$</th>
    <th>$(p \rightarrow r) \land (q \rightarrow r)$</th>
    <th>$p \vee q \rightarrow r$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
</table>
</details>
</ul>  
</details>

### Representation of If-Then as Or
$$
p \rightarrow q \equiv \neg p \vee q
$$

<details>
    <summary>Example problem</summary>

Write negations for each of the following statements:
<ol type="a">
  <li>If my car is in the repair shop, then I cannot get to class</li>
  <li>If Sara lives in Athens, then she lives in Greece</li>
</ol>  
<ul>  
  <details>
    <summary>Solution</summary>

<ol type="a">
  <li>My car is in the repair shop and I can get to class</li>
  <li>Sara lives in Athens and she does not live in Greece</li>
</ol>  
</details>
</ul>  
</details>

### Only If and the Biconditional
Given statement variables $p$ and $q$, the <strong>
biconditional of $p$ and $q$</strong> is $p$ if, and only if, $q$ and is denoted $p \leftrightarrow q$. It is true if both $p$ and $q$ have the same truth values and is false if $p$ and $q$ have opposite truth values. The words if and only if are sometimes abbreviated <strong>iff</strong>. Biconditionality indicates logical equivalence

<h3 align="center">

Truth Table for $p$ $\leftrightarrow$ $q$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$p \vee \neg q \rightarrow p$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>T</td>
  </tr>
</table>

In logical terms, $p \leftrightarrow p$ is equivalent to $(p \rightarrow q) \land (q \rightarrow p)$. This written as two conditional statements as if $p$, then $q$ and if $q$, then $p$

#### Order of Operations for Logical Operators
<ol>
  <li>

$\neg \quad \quad$ Evaluate negations first</li>
<li>

$\land, \vee \quad$ Evaluate $\land$ and $\vee$ second. When both are present, parentheses may be needed</li>
<li>

$\rightarrow$, $\leftrightarrow \quad$ Evaluate $\rightarrow$ and $\leftrightarrow$ third. When both are present, parentheses may be needed</li>
</ol>

### Necessary and Sufficient Conditions
If $r$ and $s$ are statements:

<div align="center">

$r$ is a <strong>sufficient condition</strong> for $s$ $\quad$ means $\quad$ $r$ $\rightarrow$ $s$

$r$ is a <strong>necessary condition</strong> for $s$ $\quad$ means $\quad$ $s$ $\rightarrow$ $r$

$r$ is a necessary and sufficient condition for $s$ $\quad$ means $\quad$ $r$ $\leftrightarrow$ $s$ 
</div>

<details>
    <summary>Example problem</summary>

Use truth tables to verify the following logical equivalence: $\neg(p \rightarrow q) \equiv p \land \neg q$. Include a few words of explanation with your answers
<ul>  
  <details>
    <summary>Solution</summary>

<h3 align="center">

Truth Table for $\neg(p \rightarrow q) \equiv p \land \neg q$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$\neg q$</th>
    <th>$p \rightarrow q$</th>
    <th>$\neg(p \rightarrow q)$</th>
    <th>$p \land \neg q$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
  </tr>
</table>
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Construct truth tables for the following statement: $(p \rightarrow (q \rightarrow r)) \leftrightarrow ((p \land q) \rightarrow r)$
<ul>  
  <details>
    <summary>Solution</summary>

<h3 align="center">

Truth Table for $(p \rightarrow (q \rightarrow r)) \leftrightarrow ((p \land q) \rightarrow r)$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$r$</th>
    <th>$p \land q$</th>
    <th>$q \rightarrow r$</th>
    <th>$p \rightarrow (q \rightarrow r)$</th>
    <th>$(p \land q) \rightarrow r$</th>
    <th>$(p \rightarrow (q \rightarrow r)) \leftrightarrow ((p \land q) \rightarrow r)$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
</table>
</details>
</ul>  
</details>

## Valid and Invalid Arguments
An <strong>argument</strong> is a sequence of statements, and an <strong>argument form</strong> is a sequence of statement forms. All statements in an argument and all statement forms in an argument form, except for the final one, are called <strong>premises</strong>. The final statement or statement form is called the <strong>conclusion</strong>

To say that an argument is <strong>valid</strong> means that no matter what particular statements are substituted for the statement variables in its premises, if the resulting premises are all true, then the conclusion is also true

An argument is valid if $(P$<sub>0</sub>$ + P$<sub>1</sub>$ + P$<sub>2</sub>$ \rightarrow C)$ is a tautology

An argument can be valid and if it is valid, it can potentially be sound<br />
<ul>
  <li>An argument is valid if its structure guarantees that if the premises are true, then the conclusion must be true</li>
  <li>An argument is sound if it is valid and its premises are actually true</li>
</ul>  

<details>
    <summary>Example problem</summary>

Complete the following argument to make it valid in a nontrivial way:
<ul>
  <li>If an algorithm is inefficient, then it takes too long to run</li>
  <li>If an algorithm takes too long to run, then it is not practical for large datasets</li>
  <li>

  $\therefore$</li>
</ul>

Assuming that the major (first) premise is true, what must necessarily be true for the argument to be sound?<br />

This argument form used is an example of what?
<ul>  
  <details>
    <summary>Solution</summary>

If an algorithm is inefficient, then it is not practical for large datasets<br />

This argument is an example of transitivity
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Lefty, a leader of the underworld, was killed by one of his own band of four henchmen. Detective Sharp interviewed the men and determined that all were lying except for one. He deduced who killed Lefty on the basis of the following statements:<br />
$\quad$ A. Socko: Sharky killed Lefty<br />
$\quad$ B. Fats: Muscles did not kill Lefty<br />
$\quad$ C. Sharky: Muscles was shooting craps with Socko when Lefty was knocked off<br />
$\quad$ D. Muscles: Sharky did not kill Lefty<br />

Who did kill Lefty?
<ul>  
  <details>
    <summary>Solution</summary>

Either A is true or D is true. Sharky either killed or did not kill Lefty. Assuming the Muscles was telling the truth and that Muscles killed Lefty:
<ul>
  <li>A is lie because it contradicts the truth, D</li>
  <li>B is a lie because Muscles did kill Lefty</li>
  <li>C is a lie because Muscles killed Lefty</li>
  <li>D is the truth because Sharky did not kill Lefty, Muscles did</li>
</ul>  
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Suppose the it is true that: You'll build it, but they won't come<<br >
Which of the following are then false? Select all that apply<br />
<ul>
  <li>If you build it, they will come</li>
  <li>If they come, you will build it</li>
  <li>If you won't build it, they won't come</li>
  <li>You won't build it, or they'll come</li>
  <li>If they won't come, you won't build it</li>
</ul>
<ul>  
  <details>
    <summary>Solution</summary>

The statement is $B \land \neg C$ is true when $B$ is true and when $C$ is false<br />
<ul>
  <li>

  $B \rightarrow C$: If $B$ is true and $C$ is false, this statement is false</li>
  <li>

  $C \rightarrow B$: If $B$ is true and $C$ is false, this statement is true</li>
  <li>

  $\neg B \rightarrow \neg C$: If $B$ is true and $C$ is false, this statement true</li>
  <li>

  $\neg B \vee C$: If $B$ is true and $C$ is false, this statement is false</li>
  <li>

  $\neg 
</details>
</ul>  
</details>

#### Testing an Argument Form for Validity
<ol>
  <li>Identify the premises and conclusion of the argument form</li>
  <li>Construct a truth table showing the truth values of all the premises and the conclusion</li>
  <li>A row of the truth table in which all the premises are true is called a <strong>critical row</strong>. If there is a critical row in which the conclusion is false, then it is possible for an argument of the given form to have true premises and a false conclusion, and so the argument form is invalid. If the conclusion in every critical row is true, then the argument form is valid</li>
</ol>  

<details>
    <summary>Example problem</summary>

Is the following argument form valid or invalid:<br />
$\quad q$<br />
$\quad \therefore p \vee q$
<ul>  
  <details>
    <summary>Solution</summary>
<table>
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$p \vee q$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>T</td>  
  </tr>  
  <tr>
    <td>T</td>
    <td>F</td>
    <td>T</td>  
  </tr>  
  <tr>
    <td>F</td>
    <td>T</td>
    <td>T</td>  
  </tr>  
  <tr>
    <td>F</td>
    <td>F</td>
    <td>F</td>  
  </tr>  
</table>

Note that since ($P$<sub>1</sub>) $\rightarrow C$ is a tautology as every critical row has a true conclusion, the argument is therefore valid

The column of the argument that represents the premise is: $q$<br />
The column of the argument that represents the conclusion is: $p \vee q$<br />
The argument is valid because all truth table rows that have true premises have true conclusions
</details>
</ul>  
</details>

### Modus Ponens and Modus Tollens
#### Modus Ponens
Modus Ponens is an argument of the form:

$\quad \quad$ If $p$, then $q$.<br />
$\quad \quad$ $p$.<br />
$\quad \quad \therefore q$.

Here is an example of modus ponens:<br />
$\quad \quad$ If Garrett is the best, then he will earn an A.<br />
$\quad \quad$ Garrett is the best.<br />
$\quad \quad$ Therefore, he will earn an A.

#### Modus Tollens
Modus Tollens is an argument of the form:

$\quad \quad$ If $p$, then $q$.<br />
$\quad \quad$ $\neg q$.<br />
$\quad \quad \therefore \neg p$.

Here is an example of modus tollens:<br />
$\quad \quad$ If Garrett is the best, then he will earn an A.<br />
$\quad \quad$ Garrett does not earn an A.<br />
$\quad \quad$ Therefore, Garrett is not the best.<br />

<details>
    <summary>Example problem</summary>

Consider the following arguments:<br />
$\quad$ If there are as many rational numbers as there are irrational numbers, then the set of all irrational numbers is infinite.<br />
$\quad$ The set of all irrational numbers is infinite.<br />
$\quad \therefore$ There are as many rational numbers as there are irrational numbers.
<ul>  
  <details>
    <summary>Solution</summary>

The argument is of the following form:<br />
$\quad p \rightarrow q$<br />
$\quad q$<br />
$\quad \therefore p$<br />

The argument is invalid because the consequent being true does not mean that the antecedent is true
</details>
</ul>  
</details>

### Additional Valid Argument Forms: Rules of Inference
A <strong>rule of inference</strong> is a form of argument that is valid

#### Generalization
Generalization is an argument of the form:

$\quad \quad$ $p$. $\quad \quad \quad \quad$ $q$.<br />
$\quad \quad \therefore p \vee q \quad \quad \therefore p \vee q$.

Here is an example of generalization:<br />
$\quad \quad$ $p$: Garrett is a junior.<br />
$\quad \quad$ $q$: Garrett is a senior.<br />
$\quad \quad$ Therefore, Garrett is a junior or a senior.<br />

#### Specialization
Specialization is an argument of the form:

$\quad \quad p \land q.\quad \quad p \land q$.<br />
$\quad \quad \therefore p$. $\quad \quad$ $\therefore q$.

Here is an example of specialization:<br />
$\quad \quad$ Garrett knows C++.<br />
$\quad \quad$ Garrett knows C.<br />
$\quad \quad$ Therefore, Garrett knows C++.<br />

<details>
    <summary>Example problem</summary>

Consider the following arguments:<br />
$\quad$ Sandra knows Java and Sandra knows C++.<br />
$\quad \therefore$ Sandra knows C++.
<ul>  
  <details>
    <summary>Solution</summary>

The argument is of the following form:<br />
$\quad p \land q$<br />
$\quad \therefore q$<br />

The argument is valid because one of the elements in the premise is true. If the conjunction of two elements is true, then both elements are true
</details>
</ul>  
</details>

#### Conjunction
Conjunction is an argument of the form:<br />
$\quad \quad p$<br />
$\quad \quad q$<br />
$\quad \quad \therefore p \land q$<br />

Here is an example of conjunction:<br />
$\quad \quad$ Garrett knows English.<br />
$\quad \quad$ Garrett knows Spanish<br />
$\quad \quad \therefore$ Therefore, Garrett knows English and Spanish.

#### Elimination
Elimination is an argument of the form:

$\quad \quad$ $p \vee q$ $\quad \quad p \vee q$<br />
$\quad \quad$ $\neg q. \quad \quad \quad \neg p.$<br />
$\quad \quad$ $\therefore p. \quad \quad \quad q.$<br />

Here is an example of elimination:<br />
$\quad \quad$ Garrett knows C++ or Garrett knows C.<br />
$\quad \quad$ Garrett does not know C.<br />
$\quad \quad$ Therefore, Garrett knows C++.<br />

#### Transitivity
Transitivity is an argument of the form:

$\quad \quad$ $p \rightarrow q$.<br />
$\quad \quad$ $q \rightarrow r$.<br />
$\quad \quad \therefore p \rightarrow r$.

Here is an example of transitivity:<br />
$\quad \quad$ If Garrett is 18, then he was once 17.<br />
$\quad \quad$ If Garrett is 17, then he was once 16.<br />
$\quad \quad$ Therefore, if Garrett is 18, then he was once 16.

#### Proof by Division into Cases
Proof  by division into cases is an argument of the form:<br />
$\quad \quad$ $p \vee q$.<br />
$\quad \quad$ $p \rightarrow r$.<br />
$\quad \quad$ $q \rightarrow r$.<br />
$\quad \quad \therefore r$.

Here is an example of proof by division into case:<br />
$\quad \quad$ Garrett is 18 or Garrett is 19.<br />
$\quad \quad$ If Garrett is 18, then he was once 17.<br />
$\quad \quad$ If Garrett is 19, then he was once 17.<br />
$\quad \quad$ Therefore, Garrett was once 17.

#### Contradiction
Contradiction is an argument of the form:<br />
$\quad \quad$ $\neg p \rightarrow c$<br />
$\quad \quad \therefore p.$

<details>
    <summary>Example problem</summary>

Consider the following set of premises and conclusions. Assume all variables are statement variables<br /><br />
Premises:<br />
1. $x \vee y$<br />
2. $y \rightarrow z$<br />
3. $\neg z$<br />
4. $\neg x \rightarrow w$<br />

Conclusion: $w$<br /><br />
Deduce the conclusion from the premises by applying valid argument forms
<ul>  
  <details>
    <summary>Solution</summary>

$y \rightarrow z$ 2<br />
$\neg z$ 3<br />
$\therefore \neg y$ by Modus Tollens<br />
$x \vee y$ 1<br />
$\therefore x$ by elimination<br />
$\neg x \rightarrow w$ 4<br />
$\neg x \rightarrow w \equiv (\neg x \land \neg w)' \equiv x \vee w$<br />
$\therefore w$
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Consider the following set of premises and conclusions. Assume all variables are statement variables<br /><br />
Premises:<br />
1. $p \vee q$<br />
2. $q \rightarrow r$<br />
3. $\neg p$<br />
4. $r \rightarrow s$<br />

Conclusion: $s$<br /><br />
Deduce the conclusion from the premises by applying valid argument forms
<ul>  
  <details>
    <summary>Solution</summary>

$q \rightarrow r$ 2<br />
$r \rightarrow s$ 4<br />
$\therefore s$
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Consider the following set of premises and conclusions. Assume all variables are statement variables<br /><br />
Premises:<br />
1. $m \vee n$<br />
2. $n \rightarrow (o \vee p)$<br />
3. $o \rightarrow q$<br />
4. $\neg q$<br />
5. $\neg m$<br />

Conclusion: $p$<br /><br />
Deduce the conclusion from the premises by applying valid argument forms
<ul>  
  <details>
    <summary>Solution</summary>

$o \rightarrow q$ 3<br />
$\neg q$ 4<br />
$\therefore \neg o$ by Modus Tollens<br />
$m \vee n$ 1<br />
$\neg m$ 5<br />
$\therefore n$ by elimination<br />
$n \rightarrow (o \vee p)$ 2<br />
Since $n$ is true and $o$ is false, to make premise 2 true, $p$ must be true as T $\rightarrow$ T is true<br /> 
$\therefore p$
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Given the following statements:<br />
<ol>
  <li>

  $(A \rightarrow B)$ If I finish my assignment $(A)$, then I will go to the library $(B)$</li>
  <li>

  $(B \rightarrow C)$ If I go to the library $(B)$, then I will borrow a book $(C)$</li>
  <li>

  $(\neg C)$ I did not borrow a book</li>
  <li>
  
  $(D \vee A)$ I watched a movie $(D)$ or I finished my assignment $(A)$</li>
  <li>

  $(D \vee E)$ If I watched a movie $(D)$, then I had popcorn $(E)$</li>
</ol>
Questions:<br />
<ol>
  <li>

  Did I finish my assignment $(A)$?</li>
  <li>

  Did I go to the library $(B)$?</li>
  <li>

  Did I watch a movie $(D)$</li>
  <li>

  Can we conclude that I had popcorn $(E)$</li>
</ol>    
<ul>  
  <details>
    <summary>Solution</summary>

$C$ is false<br />
$B$ must be false because since $C$ is false, then to make the statement true, $B$ must be false. This statement is vacuously true because of Modus Tollens<br />
$A$ must be false because since $B$ is false, then to make the statement true, $A$ must be false. This statement is vacuously true because of Modus Tollens<br />
Since $A$ is false, $D$ must be true by elimination<br />
$E$ must be true because if $D$ is true, then $E$ must be true to make the statement true according to Modus Ponens

<ol>
  <li>
  
  $A$: the assignment was not finished</li>
  <li>

  $B$: did not go to the library</li>
  <li>

  $D$: the movie was watched</li>
  <li>

  $E$: there was popcorn</li>
</ol>  
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Given the following statements:<br />
<ol>
  <li>

  $(X \rightarrow Y)$ If the box is in the attic $(X)$, then the ladder is in the hallway $(Y)$</li>
  <li>

  $(Y \rightarrow Z)$ If the ladder is in the hallway $(Y)$, then the door to the attic is unlocked $(Z)$</li>
  <li>

  $(Z \rightarrow W)$ If the attic door is unlocked $(Z)$, then I checked the attic $(W)$</li>
  <li>
  
  $\neg W$ I did not check the attic</li>
  <li>

  $(P \vee X)$ The box is in the basement $(P)$ or the box is in the attic $(X)$</li>
  <li>

  $(P \rightarrow Q)$ If the box is in the basement $(P)$, then the basement light is on $(Q)$</li>
  <li>

  $(\neg Q)$ The basement light is not on</li>
</ol>

Questions:<br />
<ol>
  <li>

  Is the box in the attic $(X)$?</li>
  <li>

  Is the ladder in the hallway $(Y)$?</li>
  <li>

  Is the attic door unlocked $(Z)$?</li>
  <li>
  
  Did I check the attic $(W)$?</li>
  <li>

  Is the box in the basement $(P)$?</li>
  <li>
</ol> 
<ul>  
  <details>
    <summary>Solution</summary>

$W$ is false<br />
$Z$ if false because in order for the statement to be true, $Z$ must be false according to Modus Tollens. This statement is vacuously true<br />
$Y$ is false because in order for the statement to be true, $Y$ must be false according to Modus Tollens. THis statement is vacuously true<br />
$X$ is false because in order for the statement to be true, $X$ must be false according to Modus Tollens. This statement is vacuously true<br />
$P$ must be true because according to elimination, since $X$ is false, then $P$ must be true<br />
$P$ again must be true because since $Q$ is false, then $P$ must be true<br />
$Q$ is false<br />


<ol>
  <li>
  
  $X$: the box is not in the attic</li>
  <li>

  $Y$: the ladder is not in the hallway</li>
  <li>

  $Z$: the attic door is locked</li>
  <li>

  $W$: the attic was not checked</li>
  <li>

  $P$: the box is in the basement</li>
</ol>  
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

On an island, three people are met: $A$, $B$, and $C$. They make these statements:
<ul>
  <li>
  
  $A$ says: $B$ and $C$ are of the same type</li>
  <li>

  $B$ says: $A$ is a knight</li>
  <li>

  $C$ says: $B$ is a knave</li>
</ul>

What can be concluded about $A$, $B$, $C$
<ul>  
  <details>
    <summary>Solution</summary>

$A$ has to be a knave because $B$ and $C$ cannot be of the same type. $B$ says $A$ is telling the truth and $C$ says $B$ is lying<br />
$C$ is the knight because $B$ says $A$ is a knight, which is false; therefore, $C$ is a knight and $A$ and $B$ are knaves
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

On an island, three people are met: $A$, $B$, $C$, and $D$. They make these statements:
<ul>
  <li>
  
  $A$ says: $B$ is a knave and $C$ is a knight</li>
  <li>

  $B$ says: $A$ is a knight or $D$ is a knave</li>
  <li>

  $C$ says: $D$ and I are of opposite types</li>
  <li>

  $D$ says: $C$ is a knave</li>
</ul>

What can be concluded about $A$, $B$, $C$, and $D$
<ul>  
  <details>
    <summary>Solution</summary>

$D$ is a knave<br />
$C$ is a knight<br />
$B$ is a knight<br />
$A$ is a knave<br />
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

On an island, three people are met: $A$, $B$, $C$, $D$, and $E$. They make these statements:
<ul>
  <li>
  
  $A$ says: $B$ is a knight and $C$ is a knave</li>
  <li>

  $B$ says: $C$ and $D$ are of the same type</li>
  <li>

  $C$ says: $A$ and $E$ are of opposite types</li>
  <li>

  $D$ says: $B$ is a knight or $A$ is a knave</li>
  <li>

  $E$ says: $C$ and $D$ are of different types</li>
</ul>

What can be concluded about $A$, $B$, $C$, $D$, $E$
<ul>  
  <details>
    <summary>Solution</summary>

Either $B$ is true or $E$ is true, both cannot be true<br />
If $B$ is the knave, then $C$ and $D$ are not of the same type and $E$ is true. This means $A$ is false. $D$ must be a knight. $C$ must be a knave
</details>
</ul>  
</details>

### Logical Fallacies
A <strong>fallacy</strong> is an error in reasoning that results in a faulty argument

#### Converse Error
$p \rightarrow q$<br />
$q$<br />
$\therefore p$

#### Inverse Error
$p \rightarrow q$<br />
$\neg p$<br />
$\therefore \neg q$

#### False Exclusion
$p \vee q$<br />
$p$<br />
$\therefore \neg q$

#### Other Fallacies
$p \vee q$<br />
$\therefore p$<br /><br />

$p$<br />
$\therefore p \land q$

#### Contradiction
Contradiction is an argument of the form:<br />
$\quad \quad$ $\neg p \rightarrow c$.<br />
$\quad \quad \therefore p$.

### Contrapositive
The <strong>contrapositive</strong> of the statement $p \rightarrow q$ is $\neg q \rightarrow \neg p$

<div align="center">

$\neg$ $q$ $\rightarrow$ $\neg$ $p$ $\equiv$ $\neg$ $p$ $\vee$ $q$
</div>

The contrapositive of a statement is equivalent to the original statement

<details>
    <summary>Example problem</summary>

What is the contrapositive of the statement: If $x$ is nonnegative, then $x$ is positive or $x$ is 0
<ul>  
  <details>
    <summary>Solution</summary>

If $x$ is not positive and $x$ is not zero, then $x$ is not nonnegative<br />
If $x$ is not nonnegative or $x$ is positive or $x$ is zero
</details>
</ul>  
</details>

### Converse
The <strong>converse</strong> of the statement $p \rightarrow q$ is $q \rightarrow p$

The converse of a statement is not equivalent to the original statement
<details>
    <summary>Example problem</summary>

What is the converse of the statement: If $x$ is nonnegative, then $x$ is positive or $x$ is 0
<ul>  
  <details>
    <summary>Solution</summary>

If $x$ is positive or $x$ is zero, then $x$ is nonnegative
</details>
</ul>  
</details>

### Inverse
The <strong>inverse</strong> of the statement $p \rightarrow q$ is $\neg p \rightarrow \neg q$

The inverse of a statement is not equivalent to the original statement
<details>
    <summary>Example problem</summary>

What is the inverse of the statement: If $x$ is nonnegative, then $x$ is positive or $x$ is 0
<ul>  
  <details>
    <summary>Solution</summary>

If $x$ is not nonnegative, then $x$ is not positive and $x$ is not zero
</details>
</ul>  
</details>

### Negation
The <strong>negation</strong> of the statement $p \rightarrow q$ is $\neg(p \rightarrow q)$

<div align="center">

$\neg$ $($ $p$ $\rightarrow$ $q$ $)$ $\equiv$ $p$ $\land$ $\neg$ $q$
</div>

The negation of a statement is not equivalent to the orginal statement 

<details>
    <summary>Example problem</summary>

What is the negation of the statement: If $x$ is nonnegative, then $x$ is positive or $x$ is 0
<ul>  
  <details>
    <summary>Solution</summary>

If $x$ is nonnegative and $x$ is not positive and $x$ is not zero
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Use a truth table to determine whether the argument form is valid. Indicate which columns represent the premises and which represent the conclusion, and include a sentence explaining how th truth table supports your answer<br />
$p \rightarrow q$<br />
$q \rightarrow p$<br />
$\therefore p \vee q$
<ul>  
  <details>
    <summary>Solution</summary>

<h3 align="center">

Truth Table for Argument</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$p \rightarrow q$ premises</th>
    <th>$q \rightarrow p$ premises</th>
    <th>$p \vee q$ conclusion</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
  </tr>
</table>

The argument is invalid as the premises when $p$ and $q$ are false form a critical row, but the conclusion is false; therefore, the argument is invalid 
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Use a truth table to determine whether the argument form is valid. Indicate which columns represent the premises and which represent the conclusion, and include a sentence explaining how th truth table supports your answer<br />
$p \rightarrow q \vee r$<br />
$\neg q \vee \neg r$<br />
$\therefore \neg p \vee \neg r$
<ul>  
  <details>
    <summary>Solution</summary>

<h3 align="center">

Truth Table for Argument</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$r$</th>
    <th>$\neg q$</th>
    <th>$\neg r$</th>
    <th>$q \vee r$</th>
    <th>$p \rightarrow q \vee r$ premises</th>
    <th>$\neg q \vee \neg r$ premises</th>
    <th>$\neg p \vee \neg r$ conclusion</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
  </tr>
</table>

The argument is invalid as the premises when $p$ and $r$ are true and when $q$ is false, form a critical row, but the conclusion is false; therefore, the argument is invalid 
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Prove whether the following statement is a tautology:

<div align="center">

($p$ $\rightarrow$ $q$) $\land$ ($q$ $\rightarrow$ $r$) $\rightarrow$ ($p$ $\rightarrow$ $r$)
</div>
<ul>  
  <details>
    <summary>Solution</summary>

$(\neg p \vee q) \land (\neg q \vee r) \rightarrow (\neg p \vee r)$<br />
$\neg[(\neg p \vee q) \land (\neg q \vee r)] \vee (\neg p \vee r)$<br />
$\neg(\neg p \vee q) \vee \neg(\neg q \vee r) \vee (\neg p \vee r) \quad$ De Morgan's Law<br />
$(p \land \neg q) \vee (q \land \neg r) \vee (\neg p \vee r) \quad $ De Morgan's Law<br /><br />
If $p$ is false, $(\neg p \vee r)$ is true no matter what $r$ is<br /><br />
Now, if $p$ is true:<br />
$\quad$ If $r$ is true, the expression $\neg p \vee r$ evaluates to true and the statement is true<br />
$\quad$ If $r$ is false:<br />
$\quad \quad$ If $q$ is true, the expression $q \land \neg r$ evaluates to true and the statement is true<br />
$\quad \quad$ If $q$ is false, the expression $p \land \neg q$ evaluates to true and the statement is true<br /><br />
In every possible case the expression evaluates to true, regardless of the truth values of $p$, $q$, and $r$; therefore, the statement above is a tautology
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Prove whether the following statement is a tautology:

<div align="center">

$[(p \land q) \vee (\neg p \land r)] \rightarrow [(p \vee r) \land (q \vee r)]$
</div>
<ul>  
  <details>
    <summary>Solution</summary>

$\neg[(p \land q) \vee (\neg p \land r)] \vee [(p \vee r) \land (q \vee r)] \quad$ De Morgan's Law<br />
$[\neg(p \land q) \land \neg(\neg p \land r)] \vee [(p \vee r) \land (q \vee r)] \quad$ De Morgan's Law<br />
$(\neg p \vee \neg q) \land ( p \vee \neg r) \vee (p \vee r) \land (q \vee r) \quad$ De Morgan's Law<br />
$(\neg p \vee \neg q) \land ( p \vee \neg r) \vee r \vee (p \land q) \quad$ Distributive Law<br /><br />
Now, if $p$ is true:<br />
$\quad$ If $q$ is true, then the expression $p \land q$ evaluates to true and the statement is true<br />
$\quad$ If $q$ is false:<br />
$\quad \quad$ If $r$ is true, the expression $r$ evaluates to true and the statement is true<br />
$\quad \quad$ If $r$ is false, the expression $(\neg p \vee \neg q) \land ( p \vee \neg r)$ evaluates to true and the statement is true<br /><br />
Now, if $p$ is false:<br />
$\quad$ If $q$ is true:<br />
$\quad \quad$ If $r$ is true, the expression $r$ evaluates to true and the statement is true<br />
$\quad \quad$ If $r$ is false, the expression $(\neg p \vee \neg q) \land (p \vee \neg r)$ evaluates to true and the statement is true<br />
$\quad$ If $q$ is false:
$\quad \quad$ If $r$ is true, the expression $r$ evaluates to true and the statement is true<br />
$\quad \quad$ If $r$ is false, the expression $(\neg p \vee \neg q) \land (p \vee \neg r)$ evaluates to true and the statement is true<br /><br />
For every combination of $p$, $q$, and $r$, the expression evaluates to true; therefore, the statement is a tautology
</details>
</ul>  
</details>

<details>
    <summary>Example problem</summary>

Prove whether the following statement is a tautology:

<div align="center">

$((p \rightarrow q) \land p) \rightarrow q$
</div>
<ul>  
  <details>
    <summary>Solution</summary>

$\neg ((p \rightarrow q) \land p) \vee q \quad$ De Morgan's Law<br />
$(\neg(p \rightarrow q) \vee \neg p) \vee q \quad$ De Morgan's Law<br />
$(\neg(\neg p \vee q) \vee \neg p) \vee q \quad$<br />
$((p \land \neg q) \vee \neg p) \vee q \quad$ De Morgan's Law<br /><br />
If $p$ is true:<br />
$\quad$ If $q$ is true, the expression $q$ evaluates to true and the statement is true<br />
$\quad$ If $q$ is false, the expression $(p \land \neg q)$ evaluates to true and the statement is true<br /><br />
If $p$ is false, the expression $\neg p$ evaluates to true and the statement is true<br /><br />
Since the statement evaluates to true for all combinations of $p$ and $q$, the statement is a tautology
</details>
</ul>  
</details>
