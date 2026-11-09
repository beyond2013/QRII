# Elementary Introduction to Derivatives in Mathematical Modeling

## 1. Learning Objectives

By the end of this lecture, students should be able to:

1. Explain the concept of change and rate of change using everyday examples.
2. Understand the basic meaning of a derivative.
3. Explain the relationship between derivatives and the slope of a curve.
4. Differentiate simple polynomial functions using basic differentiation rules.
5. Calculate the derivative of a function at a given value.
6. Interpret derivatives in practical situations such as speed, cost, revenue and population growth.
7. Recognize how derivatives help in mathematical modeling and decision-making.

---

## 2. Introduction: Why Do We Need Derivatives?

Consider the following situations:

- A car is travelling along a road. How fast is its speed changing?
- The population of a city is increasing. How quickly is it growing?
- A business is producing more products. How does its production cost change?
- A student is preparing for an examination. How quickly is the student's performance improving?
- A company is increasing its production. At what production level is its profit maximum?

All these situations involve something changing.

But there is an important distinction:

**Knowing that something changes is different from knowing how quickly it changes.**

For example:

Suppose a car travels 100 kilometers in 2 hours.

Its average speed is:

Average speed = Distance / Time

= 100 / 2

= 50 km/hour

This tells us the average speed during the journey.

But what if we want to know the car's speed at exactly 1:30 PM?

The average speed alone cannot tell us that.

We need a way to measure the rate of change at a particular instant.

This is where **derivatives** become useful.

### The central idea

A derivative measures how quickly one quantity changes with respect to another quantity.

For example:

- How quickly distance changes with time.
- How quickly cost changes with production.
- How quickly population changes with time.
- How quickly profit changes with sales.

In simple words:

**A derivative tells us the rate of change of something.**

---

## 3. Understanding Change Through Everyday Examples

Before introducing mathematical notation, consider the following examples.

### Example 1: Speed of a Car

Suppose a car travels:

| Time (hours) | Distance (km) |
|---|---:|
| 1 | 40 |
| 2 | 80 |
| 3 | 120 |
| 4 | 160 |

The distance increases by 40 km every hour.

Therefore:

Rate of change of distance = 40 km/hour.

This rate of change represents the speed of the car.

### Example 2: Population Growth

Suppose the population of a town changes as follows:

| Year | Population |
|---|---:|
| 2020 | 10,000 |
| 2021 | 10,500 |
| 2022 | 11,000 |
| 2023 | 11,500 |

The population increases by 500 people every year.

Therefore:

Rate of population growth = 500 people/year.

### Example 3: Production Cost

Suppose a factory produces mobile phone accessories.

Its total production cost is:

| Units Produced | Total Cost (Rs.) |
|---|---:|
| 10 | 5,000 |
| 20 | 9,000 |
| 30 | 13,000 |
| 40 | 17,000 |

Every additional 10 units increase the cost by Rs. 4,000.

The additional cost per unit is:

4,000 / 10 = Rs. 400

This is an example of a rate of change.

### Important observation

In all three examples, we are comparing two quantities:

| Situation | Changing Quantity | Reference Quantity |
|---|---|---|
| Car | Distance | Time |
| Population | Population | Time |
| Factory | Cost | Production |

Derivatives help us understand these relationships more precisely.

---

## 4. What Is a Function?

To understand derivatives, we first need to understand functions.

A function describes the relationship between an input and an output.

Consider:

y = 2x + 3

Here:

- x is the input.
- y is the output.

If x = 1:

y = 2(1) + 3 = 5

If x = 2:

y = 2(2) + 3 = 7

If x = 3:

y = 2(3) + 3 = 9

We can represent this relationship in a table:

| x | y = 2x + 3 |
|---|---:|
| 1 | 5 |
| 2 | 7 |
| 3 | 9 |
| 4 | 11 |

As x increases, y also increases.

A function is useful because it allows us to describe and predict how one quantity depends on another.

### Real-life example

Suppose the total cost of purchasing notebooks is:

C(x) = 100x

Where:

- x = Number of notebooks.
- C(x) = Total cost in rupees.

If we purchase 5 notebooks:

C(5) = 100 × 5 = Rs. 500

If we purchase 10 notebooks:

C(10) = 100 × 10 = Rs. 1,000

This is a mathematical model of the relationship between quantity and cost.

---

## 5. Understanding the Rate of Change

Suppose a student travels from home to university.

At different times, the distance covered is:

| Time (hours) | Distance (km) |
|---|---:|
| 1 | 30 |
| 2 | 60 |
| 3 | 90 |

The rate of change of distance is:

Change in distance / Change in time

Mathematically:

Rate of Change = Δy / Δx

The symbol Δ (delta) means change.

Therefore:

Δy = Change in output

Δx = Change in input

In our example:

Δy = 90 - 30 = 60

Δx = 3 - 1 = 2

Rate of change:

= 60 / 2

= 30 km/hour

### General formula

Average Rate of Change =

(Change in output) / (Change in input)

Or:

Average Rate of Change = Δy / Δx

### Practice Example

A company's revenue increases from Rs. 20,000 to Rs. 30,000 when its sales increase from 100 units to 150 units.

Calculate the average rate of change of revenue with respect to sales.

Solution:

Change in revenue = 30,000 - 20,000 = 10,000

Change in sales = 150 - 100 = 50

Average rate of change:

= 10,000 / 50

= Rs. 200 per unit

Interpretation:

For every additional unit sold, revenue increases by an average of Rs. 200 over this interval.

---

## 6. From Average Rate of Change to Instantaneous Rate of Change

This is the most important idea behind derivatives.

Consider a car travelling along a road.

Suppose we calculate its average speed between 1 PM and 2 PM.

We obtain 50 km/hour.

But the car may not have travelled at exactly 50 km/hour throughout the journey.

It might have:

- Travelled at 30 km/hour in traffic.
- Increased its speed to 70 km/hour.
- Slowed down at a traffic signal.

The average speed does not tell us the exact speed at a particular instant.

We therefore distinguish between two concepts.

### A. Average Rate of Change

Measures the change over an interval.

Example:

Average speed during a 2-hour journey.

### B. Instantaneous Rate of Change

Measures the rate of change at a particular instant.

Example:

The speed of a car at exactly 1:30 PM.

**A derivative measures the instantaneous rate of change.**

This is the fundamental idea of differentiation.

---

## 7. What Is a Derivative?

A derivative tells us how quickly a function changes at a particular point.

Suppose:

y = x²

The derivative is written as:

dy/dx

Read it as:

"Derivative of y with respect to x."

For this function:

dy/dx = 2x

This means that the rate at which y changes depends on the value of x.

Let's calculate some values.

| x | y = x² | dy/dx = 2x |
|---|---:|---:|
| 1 | 1 | 2 |
| 2 | 4 | 4 |
| 3 | 9 | 6 |
| 4 | 16 | 8 |
| 5 | 25 | 10 |

Notice that the derivative increases as x increases.

This tells us that the function is increasing more rapidly.

### Interpretation

For y = x²:

- At x = 1, the rate of change is 2.
- At x = 2, the rate of change is 4.
- At x = 3, the rate of change is 6.
- At x = 4, the rate of change is 8.

The derivative tells us the rate of change at a particular value of x.

---

## 8. Derivatives and the Slope of a Curve

You may already know that the slope of a straight line measures how steep the line is.

For a straight line:

y = mx + c

The slope is m.

For example:

y = 3x + 2

The slope is 3.

This means that whenever x increases by 1, y increases by 3.

But what happens when we have a curve instead of a straight line?

Consider:

y = x²

This is a curved graph.

Unlike a straight line, its steepness changes at different points.

At some points, the curve is relatively flat.

At other points, it becomes steeper.

The derivative measures the slope of the curve at a particular point.

### Important relationship

**The derivative of a function at a point represents the slope of the tangent line at that point.**

A tangent is a straight line that touches a curve at a particular point and represents its direction at that point.

For example:

For:

y = x²

The derivative is:

dy/dx = 2x

At x = 2:

dy/dx = 2(2) = 4

Therefore, the slope of the tangent to the curve at x = 2 is 4.

### Remember

- Positive derivative: The function is increasing.
- Negative derivative: The function is decreasing.
- Zero derivative: The tangent is horizontal at that point.

These observations will become useful when studying maximum and minimum values.

---

## 9. Basic Rules of Differentiation

We now know that a derivative measures the rate of change.

But how do we calculate it?

Let's learn a few simple rules.

### Rule 1: Derivative of a Constant

The derivative of a constant is zero.

If:

y = 5

Then:

dy/dx = 0

Why?

Because a constant does not change when x changes.

Examples:

y = 10  →  dy/dx = 0

y = 100 →  dy/dx = 0

y = -7  →  dy/dx = 0

### Rule 2: Power Rule

This is the most important rule for elementary differentiation.

If:

y = xⁿ

Then:

dy/dx = nxⁿ⁻¹

In simple words:

1. Bring the power in front as a multiplier.
2. Reduce the power by 1.

Example 1:

y = x²

dy/dx = 2x¹

Answer:

dy/dx = 2x

Example 2:

y = x³

dy/dx = 3x²

Example 3:

y = x⁴

dy/dx = 4x³

Example 4:

y = x⁵

dy/dx = 5x⁴

### Rule 3: Constant Multiple Rule

If a function is multiplied by a constant, keep the constant and differentiate the remaining function.

Example:

y = 5x²

dy/dx = 5 × 2x

Answer:

dy/dx = 10x

Another example:

y = 3x³

dy/dx = 3 × 3x²

Answer:

dy/dx = 9x²

### Rule 4: Sum and Difference Rule

Differentiate each term separately.

Example:

y = x² + 3x

dy/dx = 2x + 3

Another example:

y = 4x³ + 2x² - 5x

dy/dx = 12x² + 4x - 5

### Summary of Basic Rules

| Function | Derivative |
|---|---|
| y = 5 | 0 |
| y = x | 1 |
| y = x² | 2x |
| y = x³ | 3x² |
| y = x⁴ | 4x³ |
| y = 5x² | 10x |
| y = 3x³ | 9x² |
| y = x² + 2x | 2x + 2 |
| y = 4x³ + 3x² | 12x² + 6x |

For this introductory lecture, these rules are sufficient.

---

## 10. Solved Examples

### Example 1

Find the derivative of:

y = 3x² + 5x + 7

Solution:

Differentiate each term:

Derivative of 3x² = 6x

Derivative of 5x = 5

Derivative of 7 = 0

Therefore:

dy/dx = 6x + 5

### Example 2

Find the derivative of:

y = 4x³ - 2x² + 6x - 8

Solution:

Derivative of 4x³ = 12x²

Derivative of -2x² = -4x

Derivative of 6x = 6

Derivative of -8 = 0

Therefore:

dy/dx = 12x² - 4x + 6

### Example 3: Finding the Derivative at a Particular Point

Suppose:

y = x² + 3x

Find the derivative at x = 2.

Step 1: Differentiate.

dy/dx = 2x + 3

Step 2: Substitute x = 2.

dy/dx = 2(2) + 3

dy/dx = 4 + 3

Answer:

dy/dx = 7 at x = 2.

Interpretation:

At x = 2, the function is increasing at a rate of 7 units of y for every unit change in x, locally.

---

## 11. Applications of Derivatives in Mathematical Modeling

Derivatives become particularly useful when we apply them to real-world problems.

### Application 1: Speed and Distance

Suppose the distance travelled by a vehicle is given by:

s(t) = t² + 4t

Where:

- s = Distance in kilometers.
- t = Time in hours.

Find the speed of the vehicle at t = 3 hours.

We know:

Speed = Rate of change of distance with respect to time.

Therefore:

v(t) = ds/dt

Differentiate:

v(t) = 2t + 4

At t = 3:

v(3) = 2(3) + 4

v(3) = 10 km/hour

Answer:

The instantaneous speed at t = 3 hours is 10 km/hour.

### Application 2: Production Cost

Suppose the total cost of producing x units is:

C(x) = x² + 20x + 100

Where:

- x = Number of units produced.
- C(x) = Total production cost in rupees.

Find the rate at which production cost changes when 10 units are being produced.

Step 1: Differentiate the cost function.

C'(x) = 2x + 20

Step 2: Substitute x = 10.

C'(10) = 2(10) + 20

C'(10) = 40

Answer:

The marginal cost at a production level of 10 units is Rs. 40 per additional unit, approximately.

### What Is Marginal Cost?

Marginal cost represents the additional cost of producing one more unit.

In mathematical modeling, it is represented by the derivative of the total cost function.

Marginal Cost = C'(x)

### Application 3: Revenue and Profit

Suppose the revenue of a company is:

R(x) = 100x - 2x²

Where x represents the number of products sold.

Find the rate of change of revenue when 10 products are sold.

Step 1: Differentiate.

R'(x) = 100 - 4x

Step 2: Substitute x = 10.

R'(10) = 100 - 40

R'(10) = 60

Answer:

At 10 units, the revenue is increasing at a marginal rate of Rs. 60 per additional unit.

### Application 4: Population Growth

Suppose the population of a town is modeled by:

P(t) = 1000 + 50t + 2t²

Where:

- P(t) = Population.
- t = Number of years after 2020.

Find the population growth rate after 5 years.

Step 1: Differentiate.

P'(t) = 50 + 4t

Step 2: Substitute t = 5.

P'(5) = 50 + 4(5)

P'(5) = 70

Answer:

After 5 years, the modeled population growth rate is 70 people per year.

---

## 12. Derivatives and Optimization: Finding Maximum and Minimum

One important application of derivatives is finding maximum and minimum values.

Consider a business that wants to maximize its profit.

Suppose its profit function is:

P(x) = 40x - x²

Where x represents the number of products sold.

We want to determine the production level at which profit is maximum.

Step 1: Differentiate the profit function.

P'(x) = 40 - 2x

Step 2: Set the derivative equal to zero.

40 - 2x = 0

2x = 40

x = 20

This gives us a possible maximum or minimum point.

Step 3: Check whether it is a maximum or minimum.

The second derivative is:

P''(x) = -2

Since the second derivative is negative, the profit function has a maximum at x = 20.

Step 4: Calculate maximum profit.

P(20) = 40(20) - (20)²

P(20) = 800 - 400

P(20) = 400

Answer:

Maximum profit = 400

It occurs when 20 units are sold.

### Important Concept

When the first derivative is zero, we have a stationary point.

It may represent:

- A maximum.
- A minimum.
- A stationary point that is neither.

The second derivative helps distinguish between a maximum and minimum in simple cases.

For this introductory course, remember:

| Second Derivative | Interpretation |
|---|---|
| Positive | Local minimum |
| Negative | Local maximum |
| Zero | Further investigation is required |

---

## 13. Why Are Derivatives Important in Computer Science?

Derivatives are not limited to mathematics, physics or economics.

They are also important in computing.

### 1. Artificial Intelligence and Machine Learning
