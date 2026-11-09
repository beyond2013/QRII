# Lecture: Propositional Equivalences, Logical Fallacies, and Venn Diagrams

## 1. Introduction

Logic helps us examine statements, evaluate arguments, and determine whether conclusions follow from given information.

In previous lectures, we studied propositions, logical connectives, truth tables, and different approaches to reasoning.

This lecture extends those concepts through three important topics:

1. **Propositional Equivalences:** Understanding when two logical expressions have the same truth values.
2. **Logical Fallacies:** Identifying common errors in arguments and reasoning.
3. **Venn Diagrams:** Using diagrams to represent relationships between sets and examine logical statements.

These concepts are useful in mathematics, computer science, statistics, database systems, and everyday decision-making.

## 2. Learning Objectives

By the end of this lecture, students should be able to:

1. Explain the meaning of logical equivalence.
2. Identify and apply common laws of propositional equivalence.
3. Use truth tables to verify logical equivalences.
4. Recognize common formal and informal logical fallacies.
5. Explain how Venn diagrams represent relationships between sets.
6. Apply Venn diagrams to solve basic logical and quantitative problems.
7. Relate logical reasoning to everyday situations and computer science.

# Part A: Propositional Equivalences

## 3. What Is Logical Equivalence?

Two logical expressions are **logically equivalent** if they produce the same truth value for every possible combination of their propositions.

The symbol for logical equivalence is:

$$
\equiv
$$

For example:

$$
\neg(p \land q) \equiv (\neg p \lor \neg q)
$$

This means that the expression on the left and the expression on the right always have the same truth value.

### 3.1 Verifying Equivalence Using a Truth Table

Consider:

$$
\neg(p \land q)
$$

and

$$
\neg p \lor \neg q
$$

We can verify whether they are equivalent by constructing a truth table.

| $p$ | $q$ | $p \land q$ | $\neg(p \land q)$ | $\neg p$ | $\neg q$ | $\neg p \lor \neg q$ |
|---|---|---|---|---|---|---|
| T | T | T | F | F | F | F |
| T | F | F | T | F | T | T |
| F | T | F | T | T | F | T |
| F | F | F | T | T | T | T |

The two expressions have identical truth values in every row.

Therefore:

$$
\neg(p \land q) \equiv (\neg p \lor \neg q)
$$

This is one of De Morgan's Laws.

## 4. Important Laws of Propositional Equivalence

There are several laws that allow us to simplify or transform logical expressions without changing their truth values.

### 4.1 Identity Laws

These laws show how AND and OR behave when combined with fixed truth values.

$$
p \land T \equiv p
$$

$$
p \lor F \equiv p
$$

Example:

If $p$ is true, then $p \land T$ is also true.

If $p$ is false, then $p \land T$ is also false.

The result is always the same as $p$.

### 4.2 Domination Laws

$$
p \lor T \equiv T
$$

$$
p \land F \equiv F
$$

Explanation:

- A proposition OR true is always true.
- A proposition AND false is always false.

### 4.3 Idempotent Laws

$$
p \land p \equiv p
$$

$$
p \lor p \equiv p
$$

Repeating the same proposition does not change its truth value.

### 4.4 Double Negation Law

$$
\neg(\neg p) \equiv p
$$

Negating a proposition twice returns the original proposition.

Example:

- $p$: The computer is switched on.
- $\neg p$: The computer is not switched on.
- $\neg(\neg p)$: The computer is not not switched on.

The final statement is logically equivalent to the original proposition.

### 4.5 Commutative Laws

The order of propositions does not affect the result of AND or OR.

$$
p \land q \equiv q \land p
$$

$$
p \lor q \equiv q \lor p
$$

Example:

"A student studies AND attends classes" has the same logical meaning as "A student attends classes AND studies."

### 4.6 Associative Laws

The grouping of propositions does not affect the result when the same connective is used.

$$
(p \land q) \land r \equiv p \land (q \land r)
$$

$$
(p \lor q) \lor r \equiv p \lor (q \lor r)
$$

### 4.7 Distributive Laws

AND distributes over OR:

$$
p \land (q \lor r)
\equiv
(p \land q) \lor (p \land r)
$$

OR distributes over AND:

$$
p \lor (q \land r)
\equiv
(p \lor q) \land (p \lor r)
$$

These laws are similar to the distributive property of ordinary algebra.

For example:

$$
a(b+c)=ab+ac
$$

The logical distributive laws follow a similar pattern.

### 4.8 De Morgan's Laws

These are particularly important when negating compound expressions.

First law:

$$
\neg(p \land q)
\equiv
(\neg p \lor \neg q)
$$

Second law:

$$
\neg(p \lor q)
\equiv
(\neg p \land \neg q)
$$

In simple language:

- Negating AND changes it into OR and negates each proposition.
- Negating OR changes it into AND and negates each proposition.

**Example:**

Original statement:

"A student has passed Mathematics AND English."

Its negation is:

"The student has NOT passed Mathematics OR has NOT passed English."

The student does not need to fail both subjects for the original statement to be false. Failing either one is sufficient.

### 4.9 Implication Law

An implication can be expressed using OR and NOT.

$$
p \rightarrow q
\equiv
\neg p \lor q
$$

Example:

"If a student studies, the student is prepared."

This is logically equivalent to:

"The student does not study OR the student is prepared."

### 4.10 Contrapositive Law

An implication is logically equivalent to its contrapositive.

$$
p \rightarrow q
\equiv
\neg q \rightarrow \neg p
$$

Example:

Original:

"If a number is divisible by 4, it is even."

Contrapositive:

"If a number is not even, it is not divisible by 4."

Both statements are logically equivalent.

**Important distinction:** The converse and inverse of an implication are not generally equivalent to the original implication.

For an implication $p \rightarrow q$:

| Form | Expression |
|---|---|
| Original | $p \rightarrow q$ |
| Converse | $q \rightarrow p$ |
| Inverse | $\neg p \rightarrow \neg q$ |
| Contrapositive | $\neg q \rightarrow \neg p$ |

The original implication is equivalent to its contrapositive. The converse is equivalent to the inverse, but they are not generally equivalent to the original implication.

## 5. Simplifying Logical Expressions

Propositional equivalence laws can be used to simplify complicated expressions.

Consider:

$$
\neg(p \land q)
$$

Using De Morgan's Law:

$$
\neg p \lor \neg q
$$

The original expression has been transformed into an equivalent expression.

Another example:

$$
p \rightarrow q
$$

Using the implication law:

$$
\neg p \lor q
$$

Both expressions represent exactly the same logical condition.

### Applications in Computer Science

Logical equivalences are useful in:

- Simplifying complex conditions in programs.
- Optimizing Boolean expressions.
- Designing digital circuits.
- Constructing database queries.
- Verifying program logic.

For example, the following Python conditions are logically equivalent:

```python
if not (a and b):
    print("Condition satisfied")
```

```python
if not a or not b:
    print("Condition satisfied")
```

Both conditions execute when at least one of `a` or `b` is false.

# Part B: Logical Fallacies

## 6. What Is a Logical Fallacy?

A **logical fallacy** is an error in reasoning that makes an argument weak, misleading, or invalid.

People sometimes make arguments that sound convincing but are not supported by proper evidence or logical reasoning.

For example:

"Everyone in the class uses this mobile application. Therefore, it must be the best application."

This argument assumes that popularity proves quality. However, popularity alone does not establish that an application is the best.

Logical fallacies are important because they help us identify mistakes in arguments, advertisements, discussions, research, and everyday decisions.

## 7. Types of Logical Fallacies

Logical fallacies are commonly divided into two broad categories:

1. Formal fallacies.
2. Informal fallacies.

### 7.1 Formal Fallacies

A formal fallacy occurs when the logical structure of an argument is incorrect.

Even if the premises are true, the conclusion does not necessarily follow.

#### Example 1: Affirming the Consequent

Consider:

- If it rains, the road becomes wet.
- The road is wet.
- Therefore, it has rained.

This conclusion is not necessarily correct.

The road might be wet because someone washed it or a water pipe leaked.

Logical structure:

$$
p \rightarrow q
$$

$$
q
$$

$$
\therefore p
$$

This is a formal fallacy because the conclusion does not follow necessarily from the premises.

#### Example 2: Denying the Antecedent

Consider:

- If a student studies regularly, the student may perform well.
- The student does not study regularly.
- Therefore, the student cannot perform well.

This conclusion is not necessarily correct. The student may perform well because of prior knowledge, additional support, or other factors.

Logical structure:

$$
p \rightarrow q
$$

$$
\neg p
$$

$$
\therefore \neg q
$$

This is an invalid argument form.

### 7.2 Informal Fallacies

Informal fallacies are errors in reasoning that often involve irrelevant evidence, misleading assumptions, or weak arguments.

#### 1. Hasty Generalization

Making a general conclusion from too few examples.

Example:

"I met two students who dislike mathematics. Therefore, all students dislike mathematics."

The conclusion is based on an insufficient sample.

#### 2. False Cause

Assuming that one event caused another without sufficient evidence.

Example:

"A student started using a new notebook and obtained higher marks. Therefore, the notebook caused the improvement."

Other factors may explain the improvement.

#### 3. Ad Hominem

Attacking the person instead of addressing the person's argument.

Example:

"Your opinion about programming is wrong because you are not an experienced programmer."

The person's experience may be relevant in some contexts, but attacking the person does not establish whether the argument is correct.

#### 4. Appeal to Popularity

Assuming that something is true or correct because many people believe it.

Example:

"Most students use this website, so it must always provide accurate information."

Popularity does not guarantee accuracy.

#### 5. Appeal to Authority

Accepting a claim as true simply because a person in authority supports it, without examining the evidence.

Example:

"A famous person says that a particular diet always works. Therefore, it must be scientifically correct."

Expert opinions can be valuable, but claims still need appropriate evidence.

#### 6. False Dilemma

Presenting only two choices when other possibilities exist.

Example:

"Either you study computer science or you will never have a successful career."

There are many other educational and career paths.

#### 7. Slippery Slope

Claiming that one event will inevitably lead to a series of increasingly serious consequences without sufficient evidence.

Example:

"If students are allowed to submit one assignment late, eventually nobody will submit assignments on time."

This outcome is possible, but it is not inevitable.

#### 8. Straw Man

Misrepresenting someone's argument to make it easier to attack.

Example:

Person A: "Students should use smartphones responsibly for educational purposes."

Person B: "You want students to spend the entire lecture playing games on their phones."

Person B has changed the original argument into a different and weaker position.

## 8. Summary of Common Logical Fallacies

| Fallacy | Main error | Simple example |
|---|---|---|
| Affirming the consequent | Incorrectly concluding the condition from its result | The road is wet, so it must have rained |
| Denying the antecedent | Assuming the result cannot occur when the condition is absent | A student did not study regularly, so the student cannot pass |
| Hasty generalization | Generalizing from too few examples | Two students dislike mathematics, so everyone does |
| False cause | Assuming causation without sufficient evidence | A new notebook caused better marks |
| Ad hominem | Attacking the person instead of the argument | Your opinion is wrong because you are inexperienced |
| Appeal to popularity | Treating popularity as proof | Everyone uses it, so it must be correct |
| Appeal to authority | Treating authority as sufficient proof | A famous person said it, so it must be true |
| False dilemma | Presenting only two possible choices | Either study CS or fail in life |
| Slippery slope | Assuming an inevitable chain of consequences | One late assignment will destroy discipline |
| Straw man | Misrepresenting an argument | Changing a limited proposal into an extreme position |

## 9. Why Is Identifying Fallacies Important?

Recognizing logical fallacies helps us:

- Evaluate information critically.
- Avoid misleading advertisements.
- Identify weak arguments in discussions.
- Examine claims made on social media.
- Evaluate research conclusions.
- Make better personal and academic decisions.

A good argument should be supported by relevant evidence and sound reasoning rather than emotional language or unsupported assumptions.

# Part C: Venn Diagrams

## 10. What Is a Venn Diagram?

A **Venn diagram** is a graphical representation of sets and the relationships between them.

It normally uses circles to represent sets within a larger rectangle called the universal set.

Venn diagrams help us understand:

- Common elements between sets.
- Elements belonging to one set but not another.
- Elements belonging to either of two sets.
- Relationships between categories.
- Logical statements involving groups.

### 10.1 Basic Components

Consider a university class containing students who study Python and students who study Java.

Let:

- $U$ = All students in the class.
- $P$ = Students who study Python.
- $J$ = Students who study Java.

A Venn diagram can represent the relationship between these groups.

<diagram-placeholder />

The rectangle represents the universal set $U$, while the two circles represent sets $P$ and $J$.

The overlapping region represents students who study both Python and Java.

## 11. Basic Set Operations

Venn diagrams are commonly used to explain four basic set operations.

### 11.1 Union

The union of two sets contains all elements that belong to either set or both sets.

It is represented by:

$$
A \cup B
$$

Example:

- $A$ = Students studying Python.
- $B$ = Students studying Java.

Then $A \cup B$ represents students studying Python OR Java, including those studying both.

### 11.2 Intersection

The intersection contains elements that belong to both sets.

It is represented by:

$$
A \cap B
$$

Example:

$A \cap B$ represents students who study both Python AND Java.

### 11.3 Complement

The complement of a set contains elements in the universal set that do not belong to that set.

It is represented by:

$$
A'
$$

or

$$
A^c
$$

Example:

If $A$ represents students studying Python, then $A^c$ represents students who do not study Python.

### 11.4 Difference

The difference between two sets contains elements that belong to the first set but not the second.

It is represented by:

$$
A-B
$$

Example:

$A-B$ represents students who study Python but do not study Java.

### Summary of Set Operations

| Operation | Symbol | Meaning |
|---|---|---|
| Union | $A \cup B$ | In A OR B, including both |
| Intersection | $A \cap B$ | In both A AND B |
| Complement | $A^c$ | Not in A |
| Difference | $A-B$ | In A but not in B |

## 12. Solving Problems Using Venn Diagrams

Consider a class of 50 students.

A survey provides the following information:

- 30 students study Python.
- 25 students study Java.
- 10 students study both Python and Java.

Find:

1. How many students study only Python?
2. How many students study only Java?
3. How many students study at least one of the two languages?
4. How many students study neither language?

Let:

- $P$ = Students studying Python.
- $J$ = Students studying Java.

Given:

$$
n(U)=50
$$

$$
n(P)=30
$$

$$
n(J)=25
$$

$$
n(P \cap J)=10
$$

### Step 1: Students Studying Only Python

Subtract students studying both languages from the total studying Python.

$$
30-10=20
$$

Therefore, 20 students study only Python.

### Step 2: Students Studying Only Java

$$
25-10=15
$$

Therefore, 15 students study only Java.

### Step 3: Students Studying At Least One Language

Use the union formula:

$$
n(P \cup J)
=
n(P)+n(J)-n(P \cap J)
$$

Substituting the values:

$$
=30+25-10
$$

$$
=45
$$

Therefore, 45 students study at least one language.

### Step 4: Students Studying Neither Language

$$
50-45=5
$$

Therefore, 5 students study neither Python nor Java.

### Final Results

| Category | Number of students |
|---|---:|
| Only Python | 20 |
| Only Java | 15 |
| Both Python and Java | 10 |
| At least one language | 45 |
| Neither language | 5 |
| Total students | 50 |

## 13. Venn Diagrams and Logical Connectives

Venn diagrams can also help us understand logical operations.

Consider two sets, $A$ and $B$.

| Logical operation | Set operation | Meaning |
|---|---|---|
| AND ($\land$) | Intersection ($\cap$) | Belongs to both sets |
| OR ($\lor$) | Union ($\cup$) | Belongs to either set or both |
| NOT ($\neg$) | Complement ($^c$) | Does not belong to the set |

For example:

- $A$: Students who study Python.
- $B$: Students who study Java.

Then:

$$
A \cap B
$$

represents students studying both languages.

$$
A \cup B
$$

represents students studying at least one language.

$$
A^c
$$

represents students who do not study Python.

### 13.1 De Morgan's Laws for Sets

The logical De Morgan's Laws also have equivalent forms in set theory.

First law:

$$
(A \cup B)^c = A^c \cap B^c
$$

Second law:

$$
(A \cap B)^c = A^c \cup B^c
$$

In simple language:

- The complement of a union means being outside both sets.
- The complement of an intersection means being outside at least one of the sets.

These relationships can be verified visually using Venn diagrams.

## 14. Three-Set Venn Diagrams

Venn diagrams can represent relationships among three sets.

Consider a class of 60 students studying three subjects:

- $A$ = Mathematics.
- $B$ = Statistics.
- $C$ = Computer Science.

A three-set Venn diagram contains:

- A region belonging only to Mathematics.
- A region belonging only to Statistics.
- A region belonging only to Computer Science.
- Three pairwise overlapping regions.
- One central region representing students studying all three subjects.
- A region outside all three sets.

### 14.1 General Counting Formula

For three sets, the number of elements in their union is:

$$
\begin{aligned}
n(A \cup B \cup C) =\;& n(A)+n(B)+n(C)\\
&-n(A \cap B)-n(A \cap C)\\
&-n(B \cap C)\\
&+n(A \cap B \cap C)
\end{aligned}
$$

This formula follows the inclusion-exclusion principle.

We first add the sizes of the three sets, then subtract the pairwise intersections because they were counted twice. Finally, we add the common intersection back because it was subtracted too many times.

### Example

Suppose:

- 30 students study Mathematics.
- 28 students study Statistics.
- 25 students study Computer Science.
- 12 study both Mathematics and Statistics.
- 10 study both Mathematics and Computer Science.
- 8 study both Statistics and Computer Science.
- 5 study all three subjects.

Find the number of students studying at least one subject.

Using the formula:

$$
\begin{aligned}
n(A \cup B \cup C) =\;&30+28+25\\
&-12-10-8\\
&+5
\end{aligned}
$$

$$
=58
$$

Therefore, 58 students study at least one of the three subjects.

If the class contains 60 students, the number studying none of these subjects is:

$$
60-58=2
$$

## 15. Applications of Venn Diagrams

Venn diagrams are useful in many areas.

### 15.1 Mathematics

They help solve problems involving:

- Sets and subsets.
- Union and intersection.
- Complements.
- Inclusion-exclusion.
- Counting problems.

### 15.2 Database Systems

Consider two database tables:

- Table A contains students enrolled in Python.
- Table B contains students enrolled in Java.

A database query can identify:

- Students appearing in both tables.
- Students appearing in either table.
- Students appearing only in one table.

These operations are closely related to set operations and database joins.

### 15.3 Data Analysis

Venn diagrams can show the overlap between categories in a dataset.

For example:

- Customers who purchased laptops.
- Customers who purchased smartphones.
- Customers who purchased both.

### 15.4 Computer Science

Set theory and logical operations are used in:

- Boolean algebra.
- Search operations.
- Database queries.
- Data filtering.
- Artificial intelligence.
- Information retrieval.

## 16. Comparing the Three Topics

The three topics covered in this lecture serve different but related purposes.

| Topic | Main purpose | Common method |
|---|---|---|
| Propositional equivalences | Transform logical expressions without changing their truth values | Truth tables and equivalence laws |
| Logical fallacies | Identify errors in arguments | Critical examination of reasoning |
| Venn diagrams | Represent relationships between sets and categories | Graphical representation |

Together, they help us evaluate statements, identify errors, and represent information systematically.

## 17. Practice Exercises

### Exercise 1: Propositional Equivalences

Use logical equivalence laws to simplify the following expressions.

1. $\neg(p \land q)$
2. $\neg(p \lor q)$
3. $p \rightarrow q$
4. $\neg(\neg p)$
5. $\neg(p \land (q \lor r))$

### Exercise 2: Verify Using Truth Tables

Construct truth tables to verify the following equivalences.

1. $\neg(p \land q) \equiv \neg p \lor \neg q$
2. $\neg(p \lor q) \equiv \neg p \land \neg q$
3. $p \rightarrow q \equiv \neg p \lor q$
4. $p \rightarrow q \equiv \neg q \rightarrow \neg p$

### Exercise 3: Identify Logical Fallacies

Identify the fallacy in each statement.

1. "I met two students who failed mathematics. Therefore, all students are weak in mathematics."
2. "The road is wet, so it must have rained."
3. "Everyone is buying this mobile phone, so it must be the best."
4. "Your argument about programming is incorrect because you are a first-semester student."
5. "If we allow one student to submit an assignment late, eventually nobody will submit assignments on time."
6. "Either you study computer science or you will never have a successful career."

### Exercise 4: Venn Diagram Problems

A class contains 80 students.

- 45 students study Mathematics.
- 35 students study Statistics.
- 20 students study both subjects.

Find:

1. How many students study only Mathematics?
2. How many students study only Statistics?
3. How many students study at least one subject?
4. How many students study neither subject?

Represent the information using a Venn diagram.

### Exercise 5: Three-Set Problem

In a class of 100 students:

- 50 study Mathematics.
- 45 study Statistics.
- 40 study Computer Science.
- 20 study Mathematics and Statistics.
- 15 study Mathematics and Computer Science.
- 18 study Statistics and Computer Science.
- 10 study all three subjects.

Find:

1. How many students study at least one subject?
2. How many students study none of the three subjects?

Use the inclusion-exclusion formula.

### Exercise 6: Application-Based Questions

1. Explain how logical equivalence can help simplify a complex condition in a computer program.

2. A student claims that a particular online learning platform is the best because most students use it. Identify the possible reasoning error.

3. Explain how a Venn diagram can be used to represent students enrolled in two different programming courses.

4. Describe the relationship between logical AND and set intersection.

5. Explain why a valid argument can still have a false conclusion if one or more premises are false.

## 18. Key Takeaways

1. Logical equivalence means two expressions have identical truth values for every possible combination of propositions.
2. Equivalence laws allow us to simplify logical expressions without changing their meaning.
3. De Morgan's Laws are important for negating compound logical expressions.
4. An implication is equivalent to its contrapositive, but not generally to its converse.
5. A logical fallacy is an error in reasoning that can make an argument misleading or invalid.
6. Formal fallacies involve errors in logical structure.
7. Informal fallacies involve errors such as hasty generalization, false cause, and appeal to popularity.
8. Venn diagrams represent sets and their relationships visually.
9. Union represents OR, while intersection represents AND.
10. Complements represent elements outside a particular set.
11. The inclusion-exclusion principle helps count elements belonging to multiple sets without double-counting.
12. Logical equivalences, fallacy detection, and Venn diagrams are useful in mathematics, computing, and everyday problem-solving.

## 19. Learn and Practice Venn Lab Visually
- [Link to Venn Lab](https://beyond2013.github.io/QRII/)
