# Probabilistic Models, Bivariate Analysis, and Scatter Plots

## 1. Learning Objectives

By the end of this lecture, students should be able to:

1. Explain the concept of probability and uncertainty.
2. Calculate basic probabilities using simple formulas.
3. Understand the purpose of probabilistic models in real-life situations.
4. Explain the meaning of univariate and bivariate data.
5. Identify independent and dependent variables.
6. Understand the concept of correlation between two variables.
7. Construct and interpret scatter plots.
8. Identify positive, negative and zero correlation from scatter plots.
9. Distinguish between correlation and causation.
10. Apply basic probabilistic and bivariate analysis to practical problems.

---

# PART A: PROBABILISTIC MODELS

## 2. Introduction: Why Do We Need Probability?

Consider the following situations:

- What is the probability that it will rain tomorrow?
- What is the probability of getting heads when tossing a coin?
- What is the probability that a student will pass an examination?
- What is the probability that a customer will purchase a particular product?
- What is the probability that a computer system will experience a failure?

Notice that none of these questions can always be answered with complete certainty.

Sometimes we know what will happen. Sometimes we do not.

For example:

If you throw a stone upwards, you know it will eventually fall back to the ground.

However, if you toss a coin, you cannot know with certainty whether the result will be heads or tails.

This uncertainty is what makes probability useful.

### What Is Probability?

**Probability is a mathematical measure of how likely an event is to occur.**

It helps us describe uncertainty numerically.

Probability values range from 0 to 1.

| Probability | Meaning |
|---|---|
| 0 | Impossible event |
| 0.25 | 25% chance |
| 0.50 | 50% chance |
| 0.75 | 75% chance |
| 1 | Certain event |

For example:

- Probability of getting a 7 when rolling a standard six-sided die = 0.
- Probability of getting a number between 1 and 6 = 1.
- Probability of getting heads when tossing a fair coin = 0.5.

### Percentage Representation

Probability can also be expressed as a percentage.

For example:

0.25 = 25%

0.50 = 50%

0.75 = 75%

1.00 = 100%

Remember:

Probability of an event cannot be negative or greater than 1.

---

## 3. Basic Probability Formula

The basic formula for probability is:

**P(E) = Number of favorable outcomes / Total number of equally likely outcomes**

Where:

- P(E) = Probability of event E.
- Favorable outcomes = Outcomes we are interested in.
- Total outcomes = All possible outcomes.

### Example 1: Tossing a Coin

A fair coin has two possible outcomes:

- Heads
- Tails

What is the probability of getting heads?

Favorable outcomes = 1

Total outcomes = 2

P(Heads) = 1/2

P(Heads) = 0.5 = 50%

Therefore, the probability of getting heads is 50%.

### Example 2: Rolling a Die

A standard die has six faces:

1, 2, 3, 4, 5, 6

What is the probability of getting an even number?

Even numbers are:

2, 4, 6

Favorable outcomes = 3

Total outcomes = 6

P(Even number) = 3/6

= 1/2

= 0.5

Therefore, the probability is 50%.

### Example 3: Selecting a Student

A classroom contains 30 students:

- 18 male students.
- 12 female students.

If one student is selected randomly, what is the probability of selecting a female student?

P(Female) = 12/30

= 0.4

= 40%

Therefore, the probability of selecting a female student is 40%.

---

## 4. Important Concepts in Probability

### 4.1 Experiment

An experiment is an activity that produces an outcome.

Examples:

- Tossing a coin.
- Rolling a die.
- Selecting a student.
- Drawing a card.

### 4.2 Outcome

An outcome is a possible result of an experiment.

For a coin toss:

Heads or Tails.

For a die:

1, 2, 3, 4, 5 or 6.

### 4.3 Sample Space

The sample space is the set of all possible outcomes of an experiment.

For a coin:

S = {Heads, Tails}

For a die:

S = {1, 2, 3, 4, 5, 6}

### 4.4 Event

An event is a particular outcome or group of outcomes that we are interested in.

Example:

When rolling a die, getting an even number is an event.

E = {2, 4, 6}

### 4.5 Random Experiment

A random experiment is an experiment whose exact outcome cannot be predicted with certainty in advance.

For example, tossing a fair coin.

---

## 5. Complementary Events

Sometimes we are interested in the probability that an event will NOT happen.

For example:

What is the probability of NOT getting heads when tossing a fair coin?

We know:

P(Heads) = 0.5

Therefore:

P(Not Heads) = 1 - P(Heads)

= 1 - 0.5

= 0.5

### General Formula

**P(Not A) = 1 - P(A)**

This is called the complement rule.

### Example

The probability that a student passes an examination is 0.8.

What is the probability that the student fails?

P(Fail) = 1 - P(Pass)

= 1 - 0.8

= 0.2

Therefore, the probability of failure is 20%.

---

## 6. Independent Events

Two events are independent when the occurrence of one does not affect the probability of the other.

Example:

Tossing a coin twice.

The result of the first toss does not affect the result of the second toss.

Suppose we want to calculate the probability of getting heads in both tosses.

Probability of heads in the first toss = 1/2

Probability of heads in the second toss = 1/2

Therefore:

P(Heads and Heads) = 1/2 × 1/2

= 1/4

= 0.25

### General Formula

For two independent events A and B:

**P(A and B) = P(A) × P(B)**

### Another Example

The probability that a computer starts successfully is 0.9.

Suppose two independent computers are tested.

What is the probability that both start successfully?

P(Both successful) = 0.9 × 0.9

= 0.81

Therefore, the probability is 81%.

---

## 7. Conditional Probability: Probability Under a Given Condition

Sometimes the probability of an event changes when we receive additional information.

For example:

Suppose a university has 100 students.

- 60 students study Computer Science.
- 40 students study Information Technology.
- 30 Computer Science students are female.
- 20 Information Technology students are female.

If we randomly select a student, what is the probability of selecting a female student?

Total female students = 30 + 20 = 50.

P(Female) = 50/100 = 0.5

Now consider a different question:

**What is the probability of selecting a female student if we already know that the selected student belongs to Computer Science?**

Now we only consider the 60 Computer Science students.

Out of these, 30 are female.

Therefore:

P(Female | Computer Science) = 30/60

= 0.5

The symbol | means "given that".

### General Formula

**P(A | B) = P(A and B) / P(B)**

Where:

- A = Event of interest.
- B = Given condition.

Conditional probability is useful when decisions are made using additional information.

### Practical Applications

- Medical diagnosis.
- Fraud detection.
- Student performance analysis.
- Weather forecasting.
- Risk assessment.

---

## 8. What Are Probabilistic Models?

A probabilistic model is a mathematical representation of a situation involving uncertainty.

Instead of predicting that something will definitely happen, a probabilistic model estimates the likelihood of different outcomes.

### Example 1: Weather Forecasting

Suppose a weather forecast predicts a 70% chance of rain tomorrow.

This means the model estimates a 0.70 probability of rainfall under the forecasting conditions.

It does NOT mean that it will rain for 70% of the day.

### Example 2: Student Performance

Suppose a university analyzes previous examination results.

Based on historical information, it estimates that a student who attends at least 80% of classes has a 90% probability of passing.

This is a probabilistic prediction.

It does not guarantee that every student with 80% attendance will pass.

### Example 3: Medical Diagnosis

A medical test may indicate a high probability that a patient has a particular disease.

The result helps doctors make informed decisions.

However, probability is not certainty.

### Example 4: Artificial Intelligence

Many AI systems use probabilities to make predictions.

Examples include:

- Email spam detection.
- Speech recognition.
- Image classification.
- Recommendation systems.
- Fraud detection.

For example, an email classification system might produce:

Spam probability = 0.95

Not spam probability = 0.05

The system classifies the email as spam because the estimated probability is higher.

### Important Observation

Probabilistic models help us make decisions even when complete certainty is impossible.

---

# PART B: BIVARIATE ANALYSIS

## 9. Introduction to Data Analysis

Suppose a teacher wants to understand the academic performance of students.

The teacher collects the following information:

- Student attendance.
- Hours spent studying.
- Examination marks.
- Number of assignments completed.

There are different ways to analyze this information.

We might study one variable at a time.

For example:

What is the average examination score of the class?

Or we might study two variables together.

For example:

Is there a relationship between attendance and examination marks?

This second approach is called bivariate analysis.

### What Is Bivariate Analysis?

**Bivariate analysis is the study of the relationship between two variables.**

The word bivariate consists of:

- Bi = Two.
- Variate = Variables.

Therefore, bivariate analysis means analyzing two variables together.

### Examples

| Variable 1 | Variable 2 |
|---|---|
| Study hours | Examination marks |
| Attendance | Examination marks |
| Age | Income |
| Temperature | Electricity consumption |
| Advertising expenditure | Sales |
| Experience | Salary |

The purpose is to understand whether changes in one variable are associated with changes in another.

---

## 10. Univariate vs Bivariate Analysis

Before understanding bivariate analysis, let's distinguish it from univariate analysis.

### Univariate Analysis

Univariate analysis studies one variable at a time.

Example:

A teacher records the marks of 10 students:

50, 60, 65, 70, 75, 80, 85, 90, 55, 70

The teacher calculates:

- Average marks.
- Highest marks.
- Lowest marks.
- Distribution of marks.

Only one variable is being studied: examination marks.

### Bivariate Analysis

Now suppose the teacher records both study hours and examination marks.

| Student | Study Hours | Marks |
|---|---:|---:|
| A | 1 | 45 |
| B | 2 | 50 |
| C | 3 | 60 |
| D | 4 | 65 |
| E | 5 | 70 |
| F | 6 | 80 |

Now we are studying two variables:

1. Study hours.
2. Examination marks.

We want to understand whether study hours are related to examination performance.

This is bivariate analysis.

### Comparison

| Feature | Univariate | Bivariate |
|---|---|---|
| Number of variables | One | Two |
| Main purpose | Understand one variable | Understand relationship between two variables |
| Example | Average examination marks | Study hours vs examination marks |
| Common tools | Mean, median, mode | Correlation, scatter plots |

---

## 11. Independent and Dependent Variables

When studying the relationship between two variables, it is useful to distinguish between independent and dependent variables.

### Independent Variable

An independent variable is the variable that we use as a possible explanation or predictor.

It is commonly represented by X.

### Dependent Variable

A dependent variable is the variable whose value or behavior we want to understand or predict.

It is commonly represented by Y.

### Example 1: Study Hours and Marks

Suppose we want to investigate whether studying more hours is associated with higher examination marks.

X = Study hours

Y = Examination marks

Study hours are the independent variable.

Examination marks are the dependent variable.

### Example 2: Advertising and Sales

A company wants to understand whether advertising expenditure influences sales.

X = Advertising expenditure

Y = Sales

### Example 3: Temperature and Electricity Consumption

A researcher studies whether temperature affects electricity consumption.

X = Temperature

Y = Electricity consumption

### Important Note

Independent and dependent are roles assigned for analysis. They do not automatically prove that one variable causes the other.

---

## 12. What Is Correlation?

Suppose a teacher collects information about students' study hours and examination marks.

The data shows that students who study more hours generally obtain higher marks.

This suggests that the two variables have a positive relationship.

Such a statistical relationship is called correlation.

### Definition

**Correlation measures the strength and direction of the relationship between two variables.**

There are three basic types of correlation:

1. Positive correlation.
2. Negative correlation.
3. Zero correlation.

---

## 13. Positive Correlation

Positive correlation occurs when two variables generally move in the same direction.

When one variable increases, the other also tends to increase.

### Example

Study hours and examination marks.

| Study Hours | Marks |
|---|---:|
| 1 | 40 |
| 2 | 50 |
| 3 | 60 |
| 4 | 70 |
| 5 | 80 |

As study hours increase, marks also increase.

This is a positive correlation.

Other examples:

- Advertising expenditure and sales.
- Work experience and salary.
- Temperature and ice cream sales.

### Remember

**Positive correlation = Both variables tend to move in the same direction.**

---

## 14. Negative Correlation

Negative correlation occurs when two variables generally move in opposite directions.

When one variable increases, the other tends to decrease.

### Example

Consider the relationship between the age of a car and its market value.

| Car Age (Years) | Market Value (Rs.) |
|---|---:|
| 1 | 3,000,000 |
| 2 | 2,700,000 |
| 3 | 2,400,000 |
| 4 | 2,100,000 |
| 5 | 1,800,000 |

As the age of the car increases, its market value decreases.

This is negative correlation.

Other examples:

- Product price and demand (in many ordinary market situations).
- Speed and travel time for a fixed distance.
- Machine age and resale value.

### Remember

**Negative correlation = One variable tends to increase while the other decreases.**

---

## 15. Zero Correlation

Zero correlation means that there is no clear linear relationship between two variables.

Example:

Suppose we compare:

- Students' shoe sizes.
- Their examination marks.

There may be no meaningful relationship between these variables.

Other possible examples:

- House numbers and student marks.
- Randomly assigned identification numbers and income.

### Remember

**Zero correlation = No clear linear relationship.**

Important: Zero correlation does not necessarily mean that the variables have no relationship of any kind. They may have a nonlinear relationship.

---

# PART C: SCATTER PLOTS

## 16. What Is a Scatter Plot?

A scatter plot is a graphical representation of the relationship between two numerical variables.

Each observation is represented by a point on a graph.

One variable is plotted on the horizontal axis (X-axis).

The other variable is plotted on the vertical axis (Y-axis).

### Example

A teacher collects data about study hours and examination marks.

| Student | Study Hours (X) | Marks (Y) |
|---|---:|---:|
| A | 1 | 40 |
| B | 2 | 50 |
| C | 3 | 55 |
| D | 4 | 65 |
| E | 5 | 75 |
| F | 6 | 85 |

To create a scatter plot:

1. Draw the horizontal X-axis.
2. Draw the vertical Y-axis.
3. Label the X-axis as Study Hours.
4. Label the Y-axis as Examination Marks.
5. Plot each pair of values as a point.

For example:

Student A = (1, 40)

Student B = (2, 50)

Student C = (3, 55)

Each student contributes one point to the graph.

The resulting graph helps us visually understand the relationship between study hours and examination marks.

### Why Are Scatter Plots Useful?

Scatter plots help us:

- Identify relationships between variables.
- Recognize positive and negative correlation.
- Detect unusual observations.
- Identify possible trends.
- Understand whether a relationship is linear or nonlinear.

---

## 17. Understanding Scatter Plot Patterns

There are three basic patterns students should recognize.

### A. Positive Correlation

Points generally move upward from left to right.

As X increases, Y tends to increase.

Example:

Study hours vs examination marks.

### B. Negative Correlation

Points generally move downward from left to right.

As X increases, Y tends to decrease.

Example:

Age of a car vs resale value.

### C. No Clear Linear Correlation

Points appear randomly distributed without a clear upward or downward pattern.

Example:

Shoe size vs examination marks.

### Summary

| Correlation | Pattern | Meaning |
|---|---|---|
| Positive | Upward | Both variables tend to increase together |
| Negative | Downward | One increases while the other decreases |
| Zero | No clear linear pattern | No clear linear association |

---

## 18. Strength of Correlation

Correlation can be weak, moderate or strong.

Consider three situations.

### Strong Positive Correlation

The points are very close to an imaginary upward-sloping straight line.

This means the relationship is strongly positive.

### Weak Positive Correlation

The points generally move upward, but they are widely scattered.

The positive relationship exists, but it is weak.

### Strong Negative Correlation

The points are very close to an imaginary downward-sloping straight line.

This means the relationship is strongly negative.

### Weak Negative Correlation

The points generally move downward, but they are widely scattered.

The negative relationship is weak.

### Important Observation

The closer the points are to a straight-line pattern, the stronger the linear relationship tends to be.

---

## 19. Correlation Coefficient

We can measure correlation numerically using a value called the correlation coefficient.

It is commonly represented by the letter r.

The value of r ranges from -1 to +1.

**-1 ≤ r ≤ +1**

### Interpretation

| Correlation Coefficient | Interpretation |
|---|---|
| +1 | Perfect positive correlation |
| +0.8 | Strong positive correlation |
| +0.5 | Moderate positive correlation |
| +0.2 | Weak positive correlation |
| 0 | No linear correlation |
| -0.2 | Weak negative correlation |
| -0.5 | Moderate negative correlation |
| -0.8 | Strong negative correlation |
| -1 | Perfect negative correlation |

These numerical categories are approximate guidelines, not universal rules.

### Understanding the Extremes

If r = +1:

All observations lie exactly on an upward-sloping straight line.

If r = -1:

All observations lie exactly on a downward-sloping straight line.

If r = 0:

There is no linear correlation.

### Important Note

Students do not need to calculate the correlation coefficient manually in this introductory lecture.

The immediate objective is to understand what the values represent and how they relate to scatter plots.

---

## 20. Correlation Does Not Mean Causation

This is one of the most important concepts in statistical reasoning.

Suppose a researcher observes:

During summer:

- Ice cream sales increase.
- The number of people visiting swimming pools also increases.

There is a positive correlation between ice cream sales and swimming pool visits.

Does buying ice cream cause people to visit swimming pools?

No.

A third variable may explain both observations:

**Temperature.**

When the weather becomes hotter:

- More people buy ice cream.
- More people visit swimming pools.

Temperature influences both activities.

This demonstrates an important principle:

**Correlation does not necessarily imply causation.**

### Another Example

Suppose students who attend more classes generally obtain higher marks.

Can we conclude that attendance alone causes higher marks?

Not necessarily.

Other factors may also influence performance:

- Previous academic preparation.
- Study habits.
- Teaching quality.
- Motivation.
- Access to learning resources.

Attendance may be associated with better performance without being the only cause.

### Classroom Question

Ask students:

"If two variables increase together, can we always say that one causes the other?"

Answer: No.

We need additional evidence to establish causation.

This is particularly important when interpreting statistics in research, news reports and social media.

---

## 21. Practical Application: Student Performance Analysis

Suppose a university wants to investigate whether class attendance is associated with examination performance.

The university collects the following information:

| Student | Attendance (%) | Examination Marks |
|---|---:|---:|
| A | 40 | 35 |
| B | 50 | 45 |
| C | 60 | 50 |
| D | 65 | 60 |
| E | 70 | 65 |
| F | 80 | 75 |
| G | 90 | 85 |
| H | 95 | 90 |

Let:

X = Attendance percentage

Y = Examination marks

### Questions

1. Which variable should be placed on the X-axis?
2.
