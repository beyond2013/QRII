# Lecture: Propositions, Logical Connectives, and Truth Tables

## 1. Introduction

Logic is an important part of mathematics and computer science. It helps us determine whether statements are true or false and how different statements can be combined to form more complex statements.

In everyday life, we use logical reasoning when making decisions. For example:

- If it rains, the ground becomes wet.
- A student will pass if they obtain the required marks.
- A computer program executes an instruction only when a particular condition is true.

In mathematics and computing, we use symbols to represent statements and logical operations. This makes reasoning more precise and easier to analyze.

This lecture introduces propositions, logical connectives, and truth tables.

## 2. Learning Objectives

By the end of this lecture, students should be able to:

1. Define a proposition and distinguish it from a non-proposition.
2. Represent propositions using logical symbols.
3. Explain the main logical connectives.
4. Construct truth tables for individual and combined propositions.
5. Evaluate compound logical expressions.
6. Relate logical operations to everyday situations and computer programming.

## 3. What Is a Proposition?

A **proposition** is a declarative statement that is either true or false, but not both.

Consider the following statements:

| Statement | Proposition? | Truth value |
|---|---|---|
| Islamabad is the capital of Pakistan. | Yes | True |
| 5 is greater than 10. | Yes | False |
| 2 + 3 = 5. | Yes | True |
| Close the door. | No | Not applicable |
| What is your name? | No | Not applicable |
| This course is interesting. | Usually no | Depends on personal opinion |

A question, command, or personal opinion is generally not considered a proposition because it does not have a definite truth value.

### 3.1 Representing Propositions

We commonly use lowercase letters such as $p$, $q$, and $r$ to represent propositions.

For example:

- $p$: Islamabad is the capital of Pakistan.
- $q$: 10 is an even number.
- $r$: 7 is greater than 3.

Each proposition has one of two truth values:

- True, represented by **T** or **1**.
- False, represented by **F** or **0**.

The values 1 and 0 are particularly common in digital logic and computer systems.

## 4. What Are Logical Connectives?

Logical connectives are symbols used to combine or modify propositions.

For example, consider:

- $p$: It is raining.
- $q$: I will carry an umbrella.

We can combine these propositions in different ways:

- It is raining **and** I will carry an umbrella.
- It is raining **or** I will carry an umbrella.
- **If** it is raining, **then** I will carry an umbrella.
- It is **not** raining.

The main logical connectives are:

| Connective | Symbol | Meaning |
|---|---|---|
| Negation | $\neg$ | NOT |
| Conjunction | $\land$ | AND |
| Disjunction | $\lor$ | OR |
| Implication | $\rightarrow$ | IF...THEN |
| Biconditional | $\leftrightarrow$ | IF AND ONLY IF |

Let us examine each connective.

## 5. Negation (NOT)

Negation reverses the truth value of a proposition.

If:

$p$: It is raining.

Then:

$\neg p$: It is not raining.

The truth table for negation is:

| $p$ | $\neg p$ |
|---|---|
| T | F |
| F | T |

**Example:**

Suppose:

$p$: 8 is an even number.

Since $p$ is true, its negation is false:

$\neg p$: 8 is not an even number.

### Important Point

Negation does not necessarily mean adding the word "not" mechanically. It means expressing the logical opposite of the original statement.

For example:

- Original: All students passed.
- Negation: At least one student did not pass.

The negation is not "All students did not pass."

## 6. Conjunction (AND)

A conjunction combines two propositions using the word **AND**.

It is represented by:

$p \land q$

The conjunction is true only when **both propositions are true**.

Consider:

- $p$: A student attends the examination.
- $q$: The student submits the answer sheet.

The compound proposition is:

$p \land q$: The student attends the examination AND submits the answer sheet.

### Truth Table for AND

| $p$ | $q$ | $p \land q$ |
|---|---|---|
| T | T | T |
| T | F | F |
| F | T | F |
| F | F | F |

**Example:**

Suppose:

- $p$ = True
- $q$ = False

Then:

$p \land q = F$

The result is false because both conditions are not true.

### Remember

For AND, both conditions must be true for the complete expression to be true.

## 7. Disjunction (OR)

A disjunction combines two propositions using the word **OR**.

It is represented by:

$p \lor q$

In standard propositional logic, OR is inclusive. This means the expression is true when:

- Both propositions are true.
- Only the first proposition is true.
- Only the second proposition is true.

It is false only when both propositions are false.

### Truth Table for OR

| $p$ | $q$ | $p \lor q$ |
|---|---|---|
| T | T | T |
| T | F | T |
| F | T | T |
| F | F | F |

**Example:**

Suppose a university allows a student to qualify for a particular activity if the student:

- $p$: Has completed the required course.
- $q$: Has obtained permission from the department.

The condition is:

$p \lor q$

The condition is true if either requirement is satisfied or both are satisfied.

### Inclusive OR vs Exclusive OR

In everyday language, OR sometimes means one option but not both.

For example:

"You may choose tea or coffee."

This may imply that only one option can be selected.

However, standard logical OR ($\lor$) is inclusive. It allows both propositions to be true.

Exclusive OR, often written as XOR ($\oplus$), is true when exactly one proposition is true.

| $p$ | $q$ | $p \oplus q$ |
|---|---|---|
| T | T | F |
| T | F | T |
| F | T | T |
| F | F | F |

## 8. Implication (IF...THEN)

Implication represents a conditional statement.

It is written as:

$p \rightarrow q$

It is read as:

"If $p$, then $q$."

Here:

- $p$ is called the antecedent or hypothesis.
- $q$ is called the consequent or conclusion.

**Example:**

- $p$: A student studies regularly.
- $q$: The student is better prepared for the examination.

The implication is:

$p \rightarrow q$: If a student studies regularly, then the student is better prepared for the examination.

### Truth Table for Implication

| $p$ | $q$ | $p \rightarrow q$ |
|---|---|---|
| T | T | T |
| T | F | F |
| F | T | T |
| F | F | T |

### Understanding the Truth Table

Implication is false only when:

- The condition $p$ is true.
- The conclusion $q$ is false.

For example:

"If a student submits the assignment, the student receives marks."

If the student submits the assignment but does not receive marks, the implication is false.

In the other three cases, the implication is considered true in classical logic.

**Important:** When the condition $p$ is false, the implication is considered true regardless of the value of $q$. This may seem unusual at first, but it is the standard mathematical definition of implication.

## 9. Biconditional (IF AND ONLY IF)

A biconditional connects two propositions and indicates that each implies the other.

It is represented by:

$p \leftrightarrow q$

It is read as:

"$p$ if and only if $q$."

A biconditional is true when both propositions have the same truth value.

### Truth Table for Biconditional

| $p$ | $q$ | $p \leftrightarrow q$ |
|---|---|---|
| T | T | T |
| T | F | F |
| F | T | F |
| F | F | T |

**Example:**

Consider:

$p$: A number is divisible by 2.

$q$: A number is even.

For integers, these two statements express the same mathematical condition. Therefore, we can write:

$p \leftrightarrow q$

The biconditional is true when both statements agree in their truth values.

## 10. Summary of Logical Connectives

The following table summarizes all five major logical connectives.

| $p$ | $q$ | $\neg p$ | $p \land q$ | $p \lor q$ | $p \rightarrow q$ | $p \leftrightarrow q$ |
|---|---|---|---|---|---|---|
| T | T | F | T | T | T | T |
| T | F | F | F | T | F | F |
| F | T | T | F | T | T | F |
| F | F | T | F | F | T | T |

This is one of the most important tables in propositional logic. Students should understand the conditions under which each connective becomes true or false.

## 11. What Is a Truth Table?

A **truth table** is a systematic method of displaying the truth values of a logical expression for every possible combination of its variables.

Truth tables help us:

- Evaluate compound logical expressions.
- Check whether a logical statement is always true or always false.
- Compare two logical expressions.
- Understand the behavior of logical conditions in computer programs.

### 11.1 Number of Rows in a Truth Table

If an expression contains $n$ distinct propositions, the number of possible truth-value combinations is:

$$
\text{Number of rows} = 2^n
$$

Examples:

| Number of propositions | Calculation | Number of rows |
|---|---|---|
| 1 | $2^1$ | 2 |
| 2 | $2^2$ | 4 |
| 3 | $2^3$ | 8 |
| 4 | $2^4$ | 16 |

For example, if an expression contains three propositions $p$, $q$, and $r$, we need eight rows to represent all possible combinations.

## 12. Constructing a Truth Table for a Compound Expression

Let us evaluate the following expression:

$$
(p \land q) \lor \neg p
$$

We will use the following steps:

**Step 1:** Identify the propositions.

There are two propositions: $p$ and $q$.

Therefore, the table requires:

$$
2^2 = 4 \text{ rows}
$$

**Step 2:** List all possible combinations of $p$ and $q$.

**Step 3:** Calculate $p \land q$.

**Step 4:** Calculate $\neg p$.

**Step 5:** Calculate the final expression $(p \land q) \lor \neg p$.

### Complete Truth Table

| $p$ | $q$ | $p \land q$ | $\neg p$ | $(p \land q) \lor \neg p$ |
|---|---|---|---|---|
| T | T | T | F | T |
| T | F | F | F | F |
| F | T | F | T | T |
| F | F | F | T | T |

**Observation:** The final column gives the truth value of the complete expression for every possible combination of $p$ and $q$.

### Another Example

Construct a truth table for:

$$
(p \lor q) \land \neg q
$$

| $p$ | $q$ | $p \lor q$ | $\neg q$ | $(p \lor q) \land \neg q$ |
|---|---|---|---|---|
| T | T | T | F | F |
| T | F | T | T | T |
| F | T | T | F | F |
| F | F | F | T | F |

The final expression is true only when $p$ is true and $q$ is false.

## 13. Order of Operations in Logical Expressions

When evaluating an expression containing multiple logical connectives, we need to follow a consistent order.

A commonly used precedence order is:

1. Parentheses
2. Negation ($\neg$)
3. Conjunction ($\land$)
4. Disjunction ($\lor$)
5. Implication ($\rightarrow$)
6. Biconditional ($\leftrightarrow$)

For example:

$$
\neg p \lor q \land r
$$

The expression is interpreted as:

$$
(\neg p) \lor (q \land r)
$$

However, using parentheses is recommended because they make expressions easier to understand and avoid ambiguity.

## 14. Tautology, Contradiction, and Contingency

Truth tables can also help us classify logical expressions.

### 14.1 Tautology

A tautology is a logical expression that is always true, regardless of the truth values of its propositions.

Example:

$$
p \lor \neg p
$$

Truth table:

| $p$ | $\neg p$ | $p \lor \neg p$ |
|---|---|---|
| T | F | T |
| F | T | T |

The final column contains only T values. Therefore, the expression is a tautology.

### 14.2 Contradiction

A contradiction is a logical expression that is always false.

Example:

$$
p \land \neg p
$$

Truth table:

| $p$ | $\neg p$ | $p \land \neg p$ |
|---|---|---|
| T | F | F |
| F | T | F |

The final column contains only F values. Therefore, the expression is a contradiction.

### 14.3 Contingency

A contingency is an expression that is true for some combinations and false for others.

Example:

$$
p \land q
$$

| $p$ | $q$ | $p \land q$ |
|---|---|---|
| T | T | T |
| T | F | F |
| F | T | F |
| F | F | F |

The expression is true in one case and false in the remaining cases. Therefore, it is a contingency.

### Comparison

| Type | Meaning | Final column |
|---|---|---|
| Tautology | Always true | All T |
| Contradiction | Always false | All F |
| Contingency | Sometimes true, sometimes false | Both T and F |

## 15. Logical Equivalence

Two logical expressions are logically equivalent if they have the same truth values for every possible combination of their propositions.

The symbol used for logical equivalence is:

$$
\equiv
$$

For example, consider:

$$
\neg(p \land q) \equiv (\neg p \lor \neg q)
$$

This is known as **De Morgan's Law**.

Both expressions produce the same truth values.

| $p$ | $q$ | $\neg(p \land q)$ | $\neg p \lor \neg q$ |
|---|---|---|---|
| T | T | F | F |
| T | F | T | T |
| F | T | T | T |
| F | F | T | T |

Since both columns are identical, the expressions are logically equivalent.

Another important form of De Morgan's Law is:

$$
\neg(p \lor q) \equiv (\neg p \land \neg q)
$$

These laws are useful in mathematics, computer programming, and digital circuit design.

## 16. Applications of Logical Connectives in Computer Science

Logical connectives are widely used in computer science.

### 16.1 Conditional Statements

In programming, conditions determine which instructions should execute.

For example, in Python:

```python
marks = 65

if marks >= 50:
    print("Pass")
else:
    print("Fail")
```

The condition `marks >= 50` is either true or false.

### 16.2 Combining Conditions

Consider a university rule:

A student qualifies for a scholarship if:

- Marks are at least 80.
- Attendance is at least 75%.

In Python:

```python
marks = 85
attendance = 80

if marks >= 80 and attendance >= 75:
    print("Eligible for scholarship")
else:
    print("Not eligible")
```

The `and` operator represents logical conjunction.

### 16.3 Using OR

A student can access a computer laboratory if the student is either:

- A registered student, OR
- An authorized staff member.

```python
registered_student = False
authorized_staff = True

if registered_student or authorized_staff:
    print("Access allowed")
else:
    print("Access denied")
```

The `or` operator represents logical disjunction.

### 16.4 Using NOT

```python
is_holiday = False

if not is_holiday:
    print("University is open")
```

The `not` operator reverses a Boolean value.

**Note:** Python uses `and`, `or`, and `not` as logical operators. The values `True` and `False` represent Boolean truth values.

## 17. Practice Exercises

### Exercise 1: Identify Propositions

Identify which of the following are propositions:

1. Pakistan is in South Asia.
2. Please switch off the computer.
3. 15 is an odd number.
4. What time is the class?
5. 10 + 5 = 20.
6. Computer science is the most interesting subject.

### Exercise 2: Identify the Connective

Identify the logical connective used in each statement:

1. It is raining AND the road is wet.
2. A student passes if the student obtains at least 50 marks.
3. The computer is not switched on.
4. A student can use the lab if registered OR authorized.
5. A number is even if and only if it is divisible by 2.

### Exercise 3: Construct Basic Truth Tables

Construct truth tables for:

1. $\neg p$
2. $p \land q$
3. $p \lor q$
4. $p \rightarrow q$
5. $p \leftrightarrow q$

### Exercise 4: Evaluate Compound Expressions

Construct truth tables for the following expressions:

1. $\neg p \land q$
2. $p \lor \neg q$
3. $(p \land q) \lor \neg p$
4. $(p \lor q) \land \neg p$
5. $(p \rightarrow q) \land p$

### Exercise 5: Classify Logical Expressions

Use truth tables to determine whether each expression is a tautology, contradiction, or contingency.

1. $p \lor \neg p$
2. $p \land \neg p$
3. $p \rightarrow q$
4. $(p \land q) \rightarrow p$

### Exercise 6: Application-Based Questions

1. A student receives a certificate if the student completes the course AND passes the final examination. Represent this condition using propositions and a logical connective.

2. A computer account is unlocked if the user enters the correct password OR uses an authorized recovery method. Represent this condition logically.

3. A university is closed when it is NOT a working day. Represent this statement using a proposition and its negation.

4. A student is eligible for a laboratory examination if attendance is at least 75% AND the required assignments have been submitted. Write the logical expression.

## 18. Key Takeaways

1. A proposition is a statement that has a definite truth value: true or false.
2. Logical connectives combine or modify propositions.
3. Negation reverses the truth value of a proposition.
4. Conjunction (AND) is true only when both propositions are true.
5. Disjunction (OR) is false only when both propositions are false.
6. Implication is false only when its first proposition is true and its second proposition is false.
7. Biconditional is true when both propositions have the same truth value.
8. A truth table displays all possible truth-value combinations of a logical expression.
9. An expression containing $n$ propositions requires $2^n$ rows.
10. Logical expressions can be classified as tautologies, contradictions, or contingencies.
11. Logical operations are fundamental to programming, databases, and digital systems.

## 19. Suggested Classroom Teaching Sequence

For a three-hour lecture, the following sequence can be used:

| Time | Topic | Teaching activity |
|---|---|---|
| 20 minutes | Introduction to propositions | Ask students to identify true/false statements |
| 25 minutes | Logical connectives | Explain NOT, AND, OR using everyday examples |
| 30 minutes | Implication and biconditional | Use examination and eligibility conditions |
| 35 minutes | Basic truth tables | Construct tables on the board |
| 30 minutes | Compound expressions | Solve two expressions step by step |
| 20 minutes | Tautology, contradiction, contingency | Demonstrate using truth tables |
| 20 minutes | Practice and discussion | Students solve short exercises |

### Teaching Recommendation

Students often find implication ($\rightarrow$) confusing because it is false only in one particular case: when the first proposition is true and the second is false.

Spend extra time explaining this connective through practical examples.

For the first exercise, ask students to complete the truth tables for NOT, AND, and OR themselves. Then introduce implication and biconditional.

It is also useful to emphasize that truth tables are not merely mathematical exercises. They are the foundation of Boolean logic, conditional statements, database queries, and digital circuit design.
