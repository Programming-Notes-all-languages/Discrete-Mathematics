<details>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href='#logic-form-and-logical-equivalence'>Logic Form and Logical Equivalence</a>
  </li>
</ol>
</details>

## Logic Form and Logical Equivalence

The statement If $p$ or $q$, then $r$ can be written as:

$$
(p \vee q) \rightarrow r
$$

The contrapositive of this statement is:

$$
\neg r \rightarrow (\neg p \land \neg q)
$$

This means that if $r$ is false, then both $p$ and $q$ must be false

<ul>
  <li>An example of the above is the following: If the program syntax is faulty of or the program execution results in division by zero, then the computer will generate an error message; therefore, if the computer does not generate an error message, then the program syntax is correct and the program execution does not result in division by zero</li>
</ul>  

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
The negation of "if $p$ then $q$" is logically equivalent to: $p$ and not $q$

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
