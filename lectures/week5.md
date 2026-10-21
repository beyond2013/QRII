# Lecture: Introduction to Deterministic Models and Linear Functions in Real-World Scenarios

As part of the **Quantitative Reasoning (II)** curriculum under the HEC undergraduate policy, understanding how to apply mathematical techniques to practical situations begins with building robust, predictable frameworks[cite: 5]. This lecture introduces the fundamental concepts of deterministic modeling and linear functions, tailored specifically for second-semester undergraduate students.

---

## 1. Defining Core Terms Upfront

Before working with equations, it is essential to define what we mean by these foundational terms:

* **Model:** A simplified mathematical representation of a real-world system, process, or relationship. Instead of getting bogged down by messy real-world complexities, a model uses numbers and equations to capture the core behavior we want to study.
* **Deterministic Model:** A mathematical system or framework where every set of variable states is uniquely determined by parameters and rules, with **zero randomness or probability**[cite: 5]. If you run the model with the exact same input today, tomorrow, or a year from now, you will get the exact same output every single time. *(Contrast this with a probabilistic model, like weather forecasting, which deals with chances and likelihoods like "a 70% chance of rain".)*

---

## 2. The Mechanics of Linear Functions

A **linear function** describes a relationship where changes in one variable result in a **constant, steady rate of change** in another. 

We write this in standard slope-intercept form:
$$y = mx + c$$

* **$y$**: The dependent variable (what you are trying to calculate or predict).
* **$x$**: The independent variable (the input or driving factor you control).
* **$m$** (Slope): The constant rate of change. It tells you how much $y$ increases (or decreases) for every 1-unit increase in $x$.
* **$c$** (y-intercept): The fixed starting value or base cost when $x = 0$.

---

## 3. Step-by-Step Real-World Examples

### Example 1: Mobile Internet Data Package
Imagine a mobile network provider offers a prepaid internet package structured as follows:
* A fixed monthly subscription fee of **Rs. 300** (charged whether you use data or not).
* An additional charge of **Rs. 50 per GB** for data consumed.

We can model your total monthly phone bill ($y$) deterministically based on how many GBs you consume ($x$):
$$y = 50x + 300$$

* **If you use 0 GB ($x = 0$):**  
  $$y = 50(0) + 300 = \text{Rs. 300}$$ *(This is our fixed base cost, or $c$)*
* **If you use 4 GB ($x = 4$):**  
  $$y = 50(4) + 300 = 200 + 300 = \text{Rs. 500}$$
* **If you use 10 GB ($x = 10$):**  
  $$y = 50(10) + 300 = 500 + 300 = \text{Rs. 800}$$

**Why is this deterministic?** Because there is no guessing involved. If you consume precisely 4 GBs, the billing system follows the exact same rule every single month and outputs Rs. 500 without variation.

---

### Example 2: API Request Pricing (Tech & AI Context)
As students in Artificial Intelligence, you will frequently work with cloud services and APIs that charge based on usage. 

Suppose an AI translation API charges:
* A baseline subscription of **$10/month**.
* **$0.02** for every individual text request processed.

Our deterministic linear model for the monthly bill ($y$) given $x$ number of requests is:
$$y = 0.02x + 10$$

* If your application makes **1,000 requests** ($x = 1000$) in a month:
  $$y = 0.02(1000) + 10 = 20 + 10 = \$30$$

This allows a developer or project manager to deterministically forecast operational expenses before launching an application into production.