# Lecture: Predicates, Quantifiers, and Logic-Based Quantitative Exercises

## 1. Introduction

In our earlier discussion of logic, we learned that a proposition is a statement that can be either true or false.

For example:

- 5 is greater than 3. (True)
- 10 is less than 4. (False)
- Islamabad is the capital of Pakistan. (True)

However, some statements cannot be classified as true or false until we know more information.

Consider:

- x is greater than 5.
- Every student passed the examination.
- Some students scored more than 80 marks.
- All natural numbers are positive.

The truth of these statements depends on the value of a variable or the group of objects being discussed.

To express and analyze such statements, we use **predicates and quantifiers**.

These concepts are important in mathematics, computer science, database queries, programming, and logical reasoning.

## 2. Learning Objectives

By the end of this lecture, students should be able to:

1. Explain the meaning of a predicate.
2. Differentiate between a proposition and a predicate.
3. Understand variables and domains of discourse.
4. Explain universal and existential quantifiers.
5. Translate ordinary English statements into logical notation.
6. Negate statements containing quantifiers.
7. Use predicates and quantifiers to solve simple quantitative problems.
8. Apply logical reasoning to everyday and computing-related situations.

---

# Part A: Understanding Predicates

## 3. What Is a Predicate?

A predicate is a statement containing one or more variables that becomes either true or false when specific values are assigned to those variables.

Consider:

$$
P(x): x > 5
$$

This means:

"x is greater than 5."

The expression is not yet a proposition because we do not know the value of x.

Now assign different values:

| Value of x | Statement | Truth Value |
|---:|---|---|
| 3 | 3 > 5 | False |
| 5 | 5 > 5 | False |
| 7 | 7 > 5 | True |
| 10 | 10 > 5 | True |

We can see that the truth value changes depending on the value assigned to x.

Therefore, a predicate becomes a proposition when its variable is assigned a particular value or when the variable is quantified.

### 3.1 More Examples of Predicates

Consider the following expressions:

**Example 1:**

$$
P(x): x \text{ is an even number}
$$

- P(2) is True.
- P(5) is False.
- P(10) is True.

**Example 2:**

$$
Q(x): x^2 = 25
$$

- Q(5) is True.
- Q(-5) is True.
- Q(3) is False.

**Example 3:**

$$
R(x): x \text{ is
