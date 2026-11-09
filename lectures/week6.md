# Systems of Linear Equations and Matrix Solutions for Modeling

## 1. Introduction: Why Do We Need Systems of Equations?

Consider the following situation.

A university cafeteria sells two items:

- A sandwich costs Rs. 200.
- A cup of tea costs Rs. 100.

One student buys 2 sandwiches and 1 cup of tea and pays Rs. 500.

Another student buys 1 sandwich and 2 cups of tea and pays Rs. 400.

Suppose we do not know the individual prices of the sandwich and tea. Can we determine them from the available information?

We can represent the unknown prices using variables:

Let:

- x = Price of one sandwich
- y = Price of one cup of tea

From the first purchase:

2x + y = 500

From the second purchase:

x + 2y = 400

We now have two equations containing two unknown variables.

This is called a **system of linear equations**.

The objective is to find values of x and y that satisfy both equations simultaneously.

### Why is this useful?

Systems of equations are used in:

- Business: Calculating prices, costs and profits.
- Economics: Understanding supply and demand.
- Computer Science: Modeling problems involving multiple variables.
- Engineering: Calculating unknown quantities in interconnected systems.
- Statistics: Understanding relationships between variables.
- Everyday life: Comparing expenses, quantities and budgets.

The important idea is that sometimes one equation is not enough to solve a problem. We need multiple equations working together.

---

## 2. What Is a Linear Equation?

A linear equation is an equation in which variables have a power of 1.

Examples:

2x + 3y = 12

x + y = 10

3x - 2y = 5

These are linear equations.

The following are NOT linear equations:

x² + y = 10

xy = 20

1/x + y = 5

### How can we recognize a linear equation?

A linear equation generally has the following characteristics:

1. Variables have a power of 1.
2. Variables are not multiplied by each other.
3. Variables do not appear in denominators.
4. The equation contains constants and variable terms.

A linear equation involving two variables can be written as:

ax + by = c

Where:

- x and y are unknown variables.
- a and b are coefficients.
- c is a constant.

Example:

3x + 2y = 12

Here:

- Coefficient of x = 3
- Coefficient of y = 2
- Constant = 12

---

## 3. What Is a System of Linear Equations?

A system of linear equations consists of two or more linear equations involving the same unknown variables.

Consider:

Equation 1:

x + y = 10

Equation 2:

x - y = 2

We need to find values of x and y that satisfy BOTH equations.

Let's solve them.

Adding the two equations:

x + y = 10

x - y = 2

----------------

2x = 12

Therefore:

x = 6

Substituting x = 6 into the first equation:

6 + y = 10

y = 4

Our solution is:

x = 6, y = 4

### Verification

Always verify the solution by substituting it into the original equations.

Equation 1:

6 + 4 = 10  ✓

Equation 2:

6 - 4 = 2  ✓

Both equations are satisfied.

Therefore, the solution is correct.

**Important:** A solution to a system of equations must satisfy every equation in that system.

---

## 4. Methods for Solving Systems of Linear Equations

There are several methods for solving simultaneous linear equations.

We will discuss three basic methods.

### 4.1 Substitution Method

Consider:

x + y = 10

x - y = 2

Step 1: Take the first equation.

x + y = 10

Make x the subject:

x = 10 - y

Step 2: Substitute this expression into the second equation.

x - y = 2

(10 - y) - y = 2

10 - 2y = 2

-2y = -8

y = 4

Step 3: Substitute y = 4 into the first equation.

x + 4 = 10

x = 6

Final answer:

x = 6, y = 4

### 4.2 Elimination Method

Consider the same equations:

x + y = 10     (1)

x - y = 2      (2)

Add both equations:

    x + y = 10
    x - y = 2
    ------------
    2x = 12

Therefore:

x = 6

Substitute into equation (1):

6 + y = 10

y = 4

Final answer:

x = 6, y = 4

**Why does elimination work?**

Notice that +y and -y cancel each other when we add the equations.

This allows us to eliminate one unknown variable and solve for the other.

### 4.3 Graphical Method

A linear equation involving two variables represents a straight line on a graph.

For example:

x + y = 10

and

x - y = 2

Each equation represents a straight line.

The solution is the point where both lines intersect.

For our example:

x = 6, y = 4

Therefore, the intersection point is (6, 4).

There are three possible situations:

**Situation 1: One solution**

Two lines intersect at exactly one point.

**Situation 2: No solution**

Two lines are parallel and never intersect.

**Situation 3: Infinitely many solutions**

Both equations represent exactly the same line.

These possibilities are important because not every system of equations has exactly one solution.

---

## 5. Introduction to Matrices

So far, we have solved equations using substitution and elimination.

However, what happens when we have:

- 3 equations and 3 unknowns?
- 5 equations and 5 unknowns?
- 100 equations and 100 unknowns?

Solving large systems manually can become difficult.

This is where matrices become useful.

### What is a Matrix?

A matrix is simply a rectangular arrangement of numbers in rows and columns.

For example:

A =

| 2 | 3 |
|---|---|
| 4 | 5 |

This matrix has:

- 2 rows
- 2 columns

Therefore, its order is 2 × 2.

Another example:

B =

| 1 | 2 | 3 |
|---|---|---|
| 4 | 5 | 6 |

This matrix has 2 rows and 3 columns.

Its order is 2 × 3.

### Important Terminology

**Row:** A horizontal arrangement of numbers.

**Column:** A vertical arrangement of numbers.

**Element:** An individual number inside a matrix.

**Order:** Number of rows × number of columns.

Matrices provide an organized way to represent numerical information.

---

## 6. Representing Linear Equations Using Matrices

Consider our earlier system:

2x + y = 500

x + 2y = 400

We can separate the numbers into three matrices.

### Matrix 1: Coefficient Matrix

Take only the coefficients of the variables.

A =

| 2 | 1 |
|---|---|
| 1 | 2 |

### Matrix 2: Variable Matrix

B =

| x |
|---|
| y |

### Matrix 3: Constant Matrix

C =

| 500 |
|-----|
| 400 |

Our system can now be written as:

**AB = C**

Or:

**AX = C**

Where:

A = Coefficient matrix

X = Variable matrix

C = Constant matrix

This is called the matrix representation of a system of linear equations.

### General Form

Consider:

a1x + b1y = c1

a2x + b2y = c2

Its matrix representation is:

| a1 | b1 |
|---|---|
| a2 | b2 |

×

| x |
|---|
| y |

=

| c1 |
|---|
| c2 |

The advantage is that a system of equations can be represented in a compact mathematical form.

---

## 7. Solving Linear Equations Using Matrix Inverse

We know that:

AX = C

Our objective is to find X.

Using ordinary algebra, if:

2x = 10

Then:

x = 10/2 = 5

Similarly, for a matrix equation:

AX = C

We can multiply both sides by the inverse of matrix A.

A⁻¹AX = A⁻¹C

Since:

A⁻¹A = I

Where I is the identity matrix.

Therefore:

**X = A⁻¹C**

This is the matrix inverse method.

### What Is an Identity Matrix?

An identity matrix is a square matrix having:

- 1s along its main diagonal.
- 0s everywhere else.

For example:

I =

| 1 | 0 |
|---|---|
| 0 | 1 |

It behaves like the number 1 in ordinary multiplication.

### What Is an Inverse Matrix?

The inverse of a matrix is another matrix that produces the identity matrix when multiplied by the original matrix.

A × A⁻¹ = I

Not every matrix has an inverse.

For a 2 × 2 matrix:

A =

| a | b |
|---|---|
| c | d |

Its determinant is:

det(A) = ad - bc

If:

ad - bc ≠ 0

The matrix has an inverse.

If:

ad - bc = 0

The matrix does not have an inverse.

### Formula for a 2 × 2 Matrix Inverse

For:

A =

| a | b |
|---|---|
| c | d |

The inverse is:

A⁻¹ = 1/(ad - bc) ×

| d | -b |
|---|---|
| -c | a |

Students do not need to memorize complicated matrix operations initially. Understanding what an inverse does is more important.

---

## 8. Solved Example: Finding the Matrix Solution

Consider the system:

2x + y = 500

x + 2y = 400

Step 1: Write the coefficient matrix.

A =

| 2 | 1 |
|---|---|
| 1 | 2 |

Step 2: Write the variable matrix.

X =

| x |
|---|
| y |

Step 3: Write the constant matrix.

C =

| 500 |
|-----|
| 400 |

Therefore:

AX = C

Step 4: Calculate the determinant.

det(A) = (2 × 2) - (1 × 1)

det(A) = 4 - 1

det(A) = 3

Since the determinant is not zero, the inverse exists.

Step 5: Calculate the inverse.

A⁻¹ = 1/3 ×

| 2 | -1 |
|---|---|
| -1 | 2 |

Step 6: Calculate X.

X = A⁻¹C

Therefore:

X = 1/3 ×

| 2 | -1 |
|---|---|
| -1 | 2 |

×

| 500 |
|-----|
| 400 |

Matrix multiplication gives:

X = 1/3 ×

| (2 × 500) + (-1 × 400) |
|------------------------|
| (-1 × 500) + (2 × 400) |

X = 1/3 ×

| 600 |
|-----|
| 300 |

Therefore:

X =

| 200 |
|-----|
| 100 |

Final answer:

x = 200

y = 100

### Interpretation

Remember our original problem:

- x represented the price of a sandwich.
- y represented the price of a cup of tea.

Therefore:

Sandwich = Rs. 200

Tea = Rs. 100

We have successfully solved a real-life problem using matrices.

---

# 9. Applications: Modeling Real-Life Problems

The real importance of systems of equations is their ability to represent situations involving multiple unknown quantities.

Let's explore some examples.

### Example 1: Shopping

A shop sells notebooks and pens.

A student buys:

- 2 notebooks and 3 pens for Rs. 160.
- 3 notebooks and 2 pens for Rs. 190.

Find the price of each item.

Let:

x = Price of one notebook

y = Price of one pen

Equations:

2x + 3y = 160

3x + 2y = 190

We can solve using elimination.

Multiply the first equation by 3:

6x + 9y = 480

Multiply the second equation by 2:

6x + 4y = 380

Subtract:

5y = 100

y = 20

Substitute into the first equation:

2x + 3(20) = 160

2x + 60 = 160

2x = 100

x = 50

Answer:

Notebook = Rs. 50

Pen = Rs. 20

### Example 2: University Transportation

A university operates buses and vans.

On one trip:

- 3 buses and 2 vans carry 190 students.
- 2 buses and 3 vans carry 160 students.

Find the seating capacity of each vehicle.

Let:

x = Capacity of one bus

y = Capacity of one van

Equations:

3x + 2y = 190

2x + 3y = 160

Multiply the first equation by 3:

9x + 6y = 570

Multiply the second equation by 2:

4x + 6y = 320

Subtract:

5x = 250

x = 50

Substitute into the first equation:

3(50) + 2y = 190

150 + 2y = 190

2y = 40

y = 20

Answer:

Bus capacity = 50 students

Van capacity = 20 students

### Example 3: Business Revenue

A shop sells two products.

- Product A earns Rs. 100 profit per unit.
- Product B earns Rs. 200 profit per unit.

The shop sells 20 units in total and earns Rs. 3,000 profit.

Find how many units of each product were sold.

Let:

x = Units of Product A

y = Units of Product B

Total units:

x + y = 20

Total profit:

100x + 200y = 3000

Divide the second equation by 100:

x + 2y = 30

Now we have:

x + y = 20

x + 2y = 30

Subtract the first equation from the second:

y = 10

Therefore:

x = 10

Answer:

Product A = 10 units

Product B = 10 units

---

# 10. When Does a System Have No Solution or Many Solutions?

Consider:

x + y = 10

x + y = 15

Can both equations be true simultaneously?

No.

The same quantities cannot add up to both 10 and 15.

Therefore, this system has **no solution**.

Now consider:

x + y = 10

2x + 2y = 20

The second equation is simply twice the first equation.

Both equations represent the same relationship.

For example:

x = 4, y = 6

x = 5, y = 5

x = 8, y = 2

All satisfy both equations.

Therefore, this system has **infinitely many solutions**.

### Summary

| Situation | Meaning |
|---|---|
| One solution | A unique set of values satisfies all equations. |
| No solution | No values satisfy all equations simultaneously. |
| Infinite solutions | Many sets of values satisfy all equations. |

This is useful when analyzing whether a mathematical model provides enough information to determine unknown quantities.

---

# 11. Practice Exercises

Attempt the following exercises. Show the equations before solving them.

## Exercise A: Identify Linear Equations

Identify which of the following are linear equations.

1. 2x + 3y = 10
2. x² + y = 15
3. 5x - 2y = 8
4. xy = 20
5. 3x + 4y - 7 = 0
6. x + y² = 12

## Exercise B: Solve Using Elimination or Substitution

Solve the following systems.

**Question 1**

x + y = 12

x - y = 4

**Question 2**

2x + y = 11

x + y = 7

**Question 3**

3x + y = 13

x + y = 7

**Question 4**

2x + 3y = 16

x + y = 6

**Question 5**

3x + 2y = 16

x + 2y = 8

## Exercise C: Real-Life Modeling

**Question 1: Mobile Packages**

A student purchases two mobile packages.

- 2 basic packages and 1 premium package cost Rs. 500.
- 1 basic package and 2 premium packages cost Rs. 700.

Find the price of each package.

**Question 2: Classroom Furniture**

A university purchases chairs and tables.

- 2 tables and 3 chairs cost Rs. 16,000.
- 3 tables and 2 chairs cost Rs. 19,000.

Find the price of one table and one chair.

**Question 3: Age Problem**

The combined ages of a father and son are 50 years.

The father is 4 times as old as the son.

Find their individual ages.

**Question 4: Examination Marks**

A student obtains marks in two subjects.

The total marks are 150.

The student scores 30 marks more in Mathematics than in English.

Find the marks obtained in each subject.

## Exercise D: Matrix Representation

Convert the following systems into matrix form AX = C.

**Question 1**

2x + 3y = 12

4x + 5y = 20

**Question 2**

x + 2y = 10

3x + y = 15

**Question 3**

5x + y = 20

2x + 3y = 18

For each question, identify:

1. The coefficient matrix.
2. The variable matrix.
3. The constant matrix.
4. The order of each matrix.

## Exercise E: Matrix Inverse Practice

Consider:

A =

| 2 | 1 |
|---|---|
| 1 | 2 |

Answer the following:

1. Find the determinant of A.
2. Does the inverse of A exist?
3. Calculate A⁻¹.
4. Verify that A × A⁻¹ = I.

Now consider:

B =

| 2 | 4 |
|---|---|
| 1 | 2 |

Answer:

1. Find the determinant of B.
2. Does the inverse of B exist?
3. Explain why.

---

# 12. Short Conceptual Questions

Answer the following in your own words.

1. What is a system of linear equations?
2. Why do we sometimes need more than one equation to solve a problem?
3. What is the difference between a linear and a nonlinear equation?
4. What is a matrix?
5. What does the order of a matrix represent?
6. What is a coefficient matrix?
7. What is an identity matrix?
8. What is the purpose of finding the inverse of a matrix?
9. Can a system of equations have no solution? Explain with an example.
10. Give two examples of real-life situations that can be represented using systems of linear equations.

---

# 13. Key Takeaways

Before ending the lecture, remember these important points:

1. A linear equation contains variables with a power of 1.
2. A system of linear equations consists of multiple equations involving the same variables.
3. The solution must satisfy all equations simultaneously.
4. Substitution and elimination are basic methods of solving simultaneous equations.
5. A matrix is a rectangular arrangement of numbers in rows and columns.
6. A system of linear equations can be represented as AX = C.
7. When the coefficient matrix has an inverse, the solution is X = A⁻¹C.
8. The determinant helps determine whether the inverse exists for a square matrix.
9. Systems of equations are useful for modeling real-world situations involving multiple unknown quantities.

## Final Thought

**Mathematics is not just about finding unknown numbers. It is about building models that help us understand real-world problems.**

Systems of linear equations help us describe relationships between unknown quantities, while matrices provide an organized and efficient way to represent and solve those relationships.
