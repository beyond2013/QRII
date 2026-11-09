# Lecture: Simple Linear Regression and Correlation Analysis

## 1. Introduction

In our previous lecture, we discussed bivariate analysis and scatter plots. We learned that bivariate analysis examines the relationship between two variables.

Consider the following questions:

- Is there a relationship between the number of hours a student studies and examination marks?
- Does the price of a product affect its demand?
- Does the number of years of experience influence salary?
- Is there a relationship between distance travelled and fuel consumed?

In this lecture, we will learn two important statistical techniques:

1. **Correlation Analysis:** Measures the strength and direction of the relationship between two variables.
2. **Simple Linear Regression:** Uses the relationship between two variables to estimate or predict the value of one variable from the other.

These techniques are widely used in business, economics, education, healthcare, engineering, and data science.

## 2. Learning Objectives

By the end of this lecture, students should be able to:

1. Explain the difference between correlation and regression.
2. Interpret positive, negative, and zero correlation.
3. Understand the correlation coefficient.
4. Explain the concept of simple linear regression.
5. Identify dependent and independent variables.
6. Understand the linear regression equation.
7. Calculate simple predictions using a regression equation.
8. Recognize the limitations of correlation and regression.

---

# Part A: Correlation Analysis

## 3. What Is Correlation?

Correlation is a statistical measure that describes the direction and strength of the relationship between two numerical variables.

In simple words, correlation tells us whether two variables tend to change together.

Consider these examples:

| Variable 1 | Variable 2 | Possible Relationship |
|---|---|---|
| Study hours | Examination marks | Positive |
| Product price | Product demand | Negative |
| Outdoor temperature | Air conditioner usage | Positive |
| Shoe size | Examination marks | No meaningful relationship |

Correlation helps us understand whether changes in one variable are associated with changes in another.

### 3.1 Positive Correlation

A positive correlation exists when two variables tend to increase or decrease together.

**Example:** As the number of study hours increases, examination marks may also increase.

| Study Hours | Marks |
|---:|---:|
| 1 | 35 |
| 2 | 42 |
| 3 | 50 |
| 4 | 57 |
| 5 | 65 |

As study hours increase, marks generally increase.

**Key idea:** Both variables move in the same direction.

### 3.2 Negative Correlation

A negative correlation exists when one variable tends to increase while the other decreases.

**Example:** As the price of a product increases, its demand may decrease.

| Product Price (Rs.) | Demand (Units) |
|---:|---:|
| 100 | 90 |
| 150 | 75 |
| 200 | 60 |
| 250 | 45 |
| 300 | 30 |

As price increases, demand decreases.

**Key idea:** The variables move in opposite directions.

### 3.3 Zero or No Linear Correlation

Sometimes two variables do not show a clear linear relationship.

For example:

- A student's shoe size and examination marks.
- A person's birth month and computer programming ability.

In such cases, the correlation may be close to zero.

However, zero correlation does not always mean that two variables are completely unrelated. They may have a non-linear relationship.

## 4. The Correlation Coefficient

The correlation coefficient is a numerical value that represents the direction and strength of a linear relationship between two variables.

It is commonly represented by the symbol **r**.

Its value always lies between -1 and +1:

$$
-1 \leq r \leq +1
$$

| Correlation Coefficient | Interpretation |
|---:|---|
| +1 | Perfect positive correlation |
| +0.8 | Strong positive correlation |
| +0.5 | Moderate positive correlation |
| 0 | No linear correlation |
| -0.5 | Moderate negative correlation |
| -0.8 | Strong negative correlation |
| -1 | Perfect negative correlation |

These descriptions of strength are approximate. Their interpretation depends on the subject and context.

### Understanding the Values

- **r = +1:** Both variables have a perfect positive linear relationship.
- **r = -1:** Both variables have a perfect negative linear relationship.
- **r = 0:** No linear relationship exists.
- **r = +0.9:** A strong positive linear relationship exists.
- **r = -0.9:** A strong negative linear relationship exists.

The sign indicates the direction:

- Positive (+): Variables move in the same direction.
- Negative (-): Variables move in opposite directions.

The absolute value indicates the strength:

- Values closer to 1 indicate a stronger linear relationship.
- Values closer to 0 indicate a weaker linear relationship.

For example, -0.9 represents a stronger negative linear relationship than -0.3.

## 5. Correlation Does Not Mean Causation

This is one of the most important concepts in statistical analysis.

**Correlation does not necessarily mean that one variable causes changes in another.**

Consider the following example.

During summer:

- Ice cream sales increase.
- Cold drink sales also increase.

There may be a positive correlation between ice cream sales and cold drink sales.

Does buying ice cream cause people to buy cold drinks?

Not necessarily.

A third variable, temperature, may influence both.

This is an example of a possible third-variable explanation.

Other examples:

- Students who own expensive smartphones may have higher marks. This does not mean expensive smartphones cause better academic performance.
- People who exercise regularly may have better health. However, other factors, such as diet and lifestyle, may also contribute.

**Remember:** Correlation identifies an association. Additional evidence is required to establish causation.

---

# Part B: Simple Linear Regression

## 6. What Is Regression?

Correlation tells us whether two variables are related.

Regression goes one step further: it helps us estimate or predict the value of one variable using another variable.

For example, suppose we observe that students who study more hours generally obtain higher marks.

We may want to answer:

- What marks might a student obtain after studying for 4 hours?
- What marks might a student obtain after studying for 6 hours?
- Can we estimate examination marks using study hours?

Regression helps us answer these questions.

### Definition

Simple linear regression is a statistical technique used to describe and predict the relationship between two variables using a straight-line equation.

It involves two variables:

1. **Independent Variable (X):** The variable used to make a prediction.
2. **Dependent Variable (Y):** The variable we want to predict.

Example:

If we want to predict examination marks based on study hours:

- X = Study Hours
- Y = Examination Marks

We assume that the relationship between these variables can be reasonably represented by a straight line.

## 7. The Simple Linear Regression Equation

The general equation of a straight line is:

$$
y = mx + c
$$

In simple linear regression, we commonly write:

$$
Y = a + bX
$$

Where:

- Y = Predicted value of the dependent variable
- X = Value of the independent variable
- a = Intercept
- b = Slope

### 7.1 Understanding the Intercept (a)

The intercept represents the predicted value of Y when X is zero.

For example, consider:

$$
Y = 20 + 10X
$$

When X = 0:

$$
Y = 20 + 10(0) = 20
$$

The predicted value of Y is 20.

### 7.2 Understanding the Slope (b)

The slope tells us how much Y is expected to change when X increases by one unit.

Consider:

$$
Y = 20 + 10X
$$

The slope
