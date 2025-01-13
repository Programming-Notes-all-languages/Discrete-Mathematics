<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#logic-form-and-logical-equivalence'>Logic Form and Logical Equivalence</a>
  </li>
  <li>
    <a href='#valid-and-invalid-arguments'>Valid and Invalid Arguments</a>
  </li>
  <li>
    <a href='#digital-logic-circuits'>Digital Logic Circuits</a>
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

### Compound Statements
The <strong>negation of 
$p$</strong> is given by the following statement: $\neg p$. This $\neg$ symbol denotes $not$, meaning that $\neg p$ means "not $p$"

The <strong>
conjunction of $p$ and $q$</strong> is given by the following statement: $p \land q$. This $\land$ symbol is read as "$p$ and $q$"

The <strong>disjunction of 
$p$ and $q$</strong> is given by the following statement: $p \vee q$. This $\vee$ symbol is read as "$p$ or $q$".

In more complex statements, such as compound statements, there is an <strong>order of operations</strong> that specifies which parts of an expression are evaluated first

<ol>
  <li>

$\neg$ has the highest precedence, meaning that $\neg$ is performed first</li>

  <li>
  
The statements $\land$ and $\vee$ are coequal in order of precedence. For instance, an expression such as $p \land q \vee r$ is considered ambiguous as an expression like this must be written like $(p \land q) \vee r$ or $p \land (q \vee r)$ to have meaning</li>
</ol>

$$
p \; but \; q \quad means \quad p \; and \; q
$$

$$
neither \; p \; nor \; q \quad means \quad \neg \; p \; and \;\neg \; q
$$

<details>
    <summary>Example problem</summary>
Write each of the following sentences symbolically, letting h = "It is hot" and s = "It is sunny".<br />
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

$$
x \leq a \quad means \quad x < a \; or \; x = a
$$

$$
a \leq x \leq b \quad means \quad a \leq x \; and \; x \leq b
$$

<details>
    <summary>Example problem</summary>

Suppose $x$ is a particular real number. Let $p$, $q$, and $r$ symbolize "0 < $x$", "$x$ < 3", and "$x$ = 3", respectively. Write the following inequalities symbolically:<br />
a) $x \leq $ 3<br />
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

### The Negation of a Conditional Statement
The negation of "if $p$ then $q$" is logically equivalent to "$p$ and not $q$"

This can be restated symbolically as the following:

$$
\neg(p \rightarrow q) \equiv p \land \neg q
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

### The contrapositive of a Conditional Statement

The <strong>contrapositive</strong> of a conditional statement of the form "if $p$ then $q$" is if $\neg q$ then $\neg p$. Symbolically, the contrapositive of $p \rightarrow q$ is $\neg q \rightarrow \neg p$

### The Converse and Inverse of a Conditional Statement
Suppose a conditional statement of the form "If $p$ then $q$" is given:

1. The <strong>converse</strong> is "If $q$ then $p$"</li>
2. The <strong>inverse</strong> is "If $\neg p$ then $\neg q$  

Symbolically,
the converse of $p \rightarrow q$ is $q \rightarrow p$ and the inverse of $p \rightarrow q$ is $\neg p \rightarrow \neg q$

### Only If and the Biconditional
Given statement variables $p$ and $q$, the <strong>
biconditional of $p$ and $q$</strong> is "$p$ if, and only if, $q$" and is denoted $p \leftrightarrow q$. It is true if both $p$ and $q$ have the same truth values and is false if $p$ and $q$ have opposite truth values. The words if and only if are sometimes abbreviated <strong>iff</strong>. Biconditionality indicates logical equivalence

<h3 align="center">

Truth Table for $p \leftrightarrow q$</h3>
<table align="center">
  <tr>
    <th>$p$</th>
    <th>$q$</th>
    <th>$p \vee \neg q \rightarrow p$</th>
  </tr>
  <tr>
    <td>T</td>
    <td>T</td>
    <td>F</td>
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

$r$ is a <strong>sufficient condition</strong> for $s \quad$ means $\quad$ "if $r$ then $s$"

$r$ is a <strong>necessary condition</strong> for $s \quad$ means $\quad$ "if not $r$ then not $s$
</div>

In other words, to say "$r$ is a sufficient condition for $s$ means that the occurrence of $r$ guarantees the occurrence of $s$. However, to say "$r$ is a necessary condition for $s$" means that if $r$ does not occur, then $s$ cannot occur either

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
    <td>F</td>
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
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
  </tr>
  <tr>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>T</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
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
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>T</td>
    <td>T</td>
    <td>T</td>
    <td>F</td>
  </tr>
</table>
</details>
</ul>  
</details>

## Valid and Invalid Arguments
An <strong>argument</strong> is a sequence of statements, and an <strong>argument form</strong> is a sequence of statement forms. All statements in an argument and all statement forms in an argument form, except for the final one, are called <strong>premises</strong>. The final statement or statement form is called the <strong>conclusion</strong>

To say that an argument is <strong>valid</strong> means that no matter what particular statements are substituted for the statement variables in its premises, if the resulting premises are all true, then the conclusion is also true

#### Testing an Argument Form for Validity
<ol>
  <li>Identify the premises and conclusion of the argument form</li>
  <li>Construct a truth table showing the truth values of all the premises and the conclusion</li>
  <li>A row of the truth table in which all the premises are true is called a <strong>critical row</strong>. If there is a critical row in which the conclusion is false, then it is possible for an argument of the given form to have true premises and a false conclusion, and so the argument form is invalid. If the conclusion in every critical row is true, then the argument form is valid</li>
</ol>  

### Modus Ponens and Modus Tollens
#### Modus Ponens
Modus Ponens is an argument of the form:

$\quad \quad$ If $p$, then $q$.<br />
$\quad \quad$ $p$.<br />
$\quad \quad$ $\therefore q$.

Here is an example of modus ponens:<br />
$\quad \quad$ If Garrett is the best, then he will earn an A.<br />
$\quad \quad$ Garrett is the best.<br />
$\quad \quad$ Therefore, he will earn an A.

#### Modus Tollens
Modus Tollens is an argument of the form:

$\quad \quad$ If $p$, then $q$.<br />
$\quad \quad$ $\neg q$.<br />
$\quad \quad$ $\therefore \neg p$.

Here is an example of modus tollens:<br />
$\quad \quad$ If Garrett is the best, then he will earn an A.<br />
$\quad \quad$ Garrett does not earn an A.<br />
$\quad \quad$ Therefore, Garrett is not the best.<br />

### Additional Valid Argument Forms: Rules of Inference
A <strong>rule of inference</strong> is a form of argument that is valid

#### Generalization
Generalization is an argument of the form:

$\quad \quad$ $p$. $\quad \quad \quad \quad$ $q$.<br />
$\quad \quad$ $\therefore p \vee q \quad \quad$ $\therefore p \vee q$.

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

#### Elimination
Elimination is an argument of the form:

$\quad \quad$ $p \vee q$.<br />
$\quad \quad$ $\neg q$.<br />
$\quad \quad$ $\therefore p$.

Here is an example of elimination:<br />
$\quad \quad$ Garrett knows C++ or Garrett knows C.<br />
$\quad \quad$ Garrett does not know C.<br />
$\quad \quad$ Therefore, Garrett knows C++.<br />

#### Transitivity
Transitivity is an argument of the form:

$\quad \quad$ $p \rightarrow q$.<br />
$\quad \quad$ $q \rightarrow r$.<br />
$\quad \quad$ $\therefore p \rightarrow r$.

Here is an example of transitivity:<br />
$\quad \quad$ If Garrett is 18, then he was once 17.<br />
$\quad \quad$ If Garrett is 17, then he was once 16.<br />
$\quad \quad$ Therefore, if Garrett is 18, then he was once 16.

#### Proof by Division into Cases
Proof  by division into cases is an argument of the form:<br />
$\quad \quad$ $p \vee q$.<br />
$\quad \quad$ $p \rightarrow r$.<br />
$\quad \quad$ $q \rightarrow r$.<br />
$\quad \quad$ $\therefore r$.

Here is an example of proof by division into case:<br />
$\quad \quad$ Garrett is 18 or Garrett is 19.<br />
$\quad \quad$ If Garrett is 18, then he was once 17.<br />
$\quad \quad$ If Garrett is 19, then he was once 17.<br />
$\quad \quad$ Therefore, Garrett was once 17.

#### Contradiction
Contradiction is an argument of the form:<br />
$\quad \quad$ $\neg p \rightarrow c$.<br />
$\quad \quad$ $\therefore p$.

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

## Digital Logic Circuits
<table>
    <thead>
        <tr>
            <th>Gate</th>
            <th>Symbol</th>
            <th>Truth Table</th>
        </tr>
    </thead>
    <tbody>
        <!-- AND Gate -->
        <tr>
            <td>AND</td>
            <td><img src="Images/Logic Gates/AND.png" alt="AND Gate Symbol" width="120" height="50"></td>
            <td>
                <table>
                    <tr><td>0</td><td>0</td><td>0</td></tr>
                    <tr><td>0</td><td>1</td><td>0</td></tr>
                    <tr><td>1</td><td>0</td><td>0</td></tr>
                    <tr><td>1</td><td>1</td><td>1</td></tr>
                </table>
            </td>
        </tr>
        <!-- OR Gate -->
        <tr>
            <td>OR</td>
            <td><img src="Images/Logic Gates/OR.png" alt="OR Gate Symbol" width="120" height="50"></td>
            <td>
                <table>
                    <tr><td>0</td><td>0</td><td>0</td></tr>
                    <tr><td>0</td><td>1</td><td>1</td></tr>
                    <tr><td>1</td><td>0</td><td>1</td></tr>
                    <tr><td>1</td><td>1</td><td>1</td></tr>
                </table>
            </td>
        </tr>
        <!-- NOT Gate -->
        <tr>
            <td>NOT</td>
            <td><img src="Images/Logic Gates/NOT.png" alt="NOT Gate Symbol" width="120" height="50"></td>
            <td>
                <table>
                    <tr><td>0</td><td>1</td></tr>
                    <tr><td>1</td><td>0</td></tr>
                </table>
            </td>
        </tr>
        <!-- NAND Gate -->
        <tr>
            <td>NAND</td>
            <td><img src="Images/Logic Gates/NAND.png" alt="NAND Gate Symbol" width="120" height="50"></td>
            <td>
                <table>
                    <tr><td>0</td><td>0</td><td>1</td></tr>
                    <tr><td>0</td><td>1</td><td>1</td></tr>
                    <tr><td>1</td><td>0</td><td>1</td></tr>
                    <tr><td>1</td><td>1</td><td>0</td></tr>
                </table>
            </td>
        </tr>
        <!-- NOR Gate -->
        <tr>
            <td>NOR</td>
            <td><img src="Images/Logic Gates/NOR.png" alt="NOR Gate Symbol" width="120" height="50"></td>
            <td>
                <table>
                    <tr><td>0</td><td>0</td><td>1</td></tr>
                    <tr><td>0</td><td>1</td><td>0</td></tr>
                    <tr><td>1</td><td>0</td><td>0</td></tr>
                    <tr><td>1</td><td>1</td><td>0</td></tr>
                </table>
            </td>
        </tr>
    </tbody>
</table>
