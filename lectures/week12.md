# Lecture: Estimation, Confidence Intervals, Hypothesis Testing, and Statistical Inference

## 1. Introduction

In statistics, we often want to understand an entire population, but collecting information from every member of that population may be difficult, expensive, or time-consuming.

For example:

- A university wants to know the average marks of all BS students.
- A hospital wants to estimate the average recovery time of patients.
- A company wants to know the average monthly income of its customers.
- A researcher wants to determine whether a new teaching method improves student performance.

Instead of collecting information from everyone, we can select a smaller group called a **sample** and use its information to draw conclusions about the entire population.

This process is called **statistical inference**.

In this lecture, we will study four important concepts:

1. Estimation
2. Confidence Intervals
3. Hypothesis Testing
4. Statistical Inference using z-tests and t-tests

These techniques are widely used in research, business, healthcare, education, and data science.

## 2. Learning Objectives

By the end of this lecture, students should be able to:

1. Differentiate between a population and a sample.
2. Explain the purpose of statistical estimation.
3. Understand point estimates and interval estimates.
4. Interpret confidence intervals.
5. Explain the purpose of hypothesis testing.
6. Understand null and alternative hypotheses.
7. Describe the basic idea of z-tests and t-tests.
8. Interpret p-values and significance levels.
9. Understand how statistical inference supports decision-making.

---

# Part A: Population, Sample, and Estimation

## 3. Population and Sample

Before understanding estimation, we need to distinguish between two important terms.

### 3.1 Population

A population is the complete group of individuals, objects, or observations that we want to study.

Examples:

- All students enrolled in a university.
- All registered vehicles in a city.
- All customers of a bank.
- All computers in a laboratory.

### 3.2 Sample

A sample is a smaller group selected from the population for analysis.

For example:

Suppose a university has 10,000 students. We select 200 students and record their examination marks.

- Population = All 10,000 students.
- Sample = The selected 200 students.

We study the sample because collecting information from all 10,000 students may require considerable time and effort.

### 3.3 Why Do We Use Samples?

Sampling helps us:

- Save time.
- Reduce research costs.
- Make data collection manageable.
- Study large populations.
- Make informed decisions using limited information.

However, a sample should represent the population reasonably well. A biased or poorly selected sample may lead to misleading conclusions.

## 4. What Is Estimation?

Estimation is the process of using sample data to approximate an unknown value of a population.

For example:

Suppose we want to know the average examination marks of all students in a university.

Instead of calculating the average marks of every student, we select a sample of 100 students.

If the average marks of these 100 students are 68, we may use 68 as an estimate of the university-wide average.

The actual population average may be different, but our sample provides useful information.

### 4.1 Population Parameter and Sample Statistic

Two terms are important in estimation:

**Population Parameter:** A numerical value describing an entire population.

**Sample Statistic:** A numerical value calculated from a sample.

For example:

| Population | Sample |
|---|---|
| Population mean (μ) | Sample mean (x̄) |
| Population proportion (p) | Sample proportion (p̂) |
| Population standard deviation (σ) | Sample standard deviation (s) |

The Greek symbols commonly represent population parameters, while Roman symbols commonly represent sample statistics.

### 4.2 Point Estimation

Point estimation provides a single numerical value as an estimate of an unknown population parameter.

Example:

Suppose the average marks of a sample of 50 students are 72.

We use this value to estimate the population average.

$$
\bar{x} = 72
$$

Here:

- x̄ = Sample mean.
- 72 = Estimated population mean.

This is called a point estimate because it gives one specific value.

### 4.3 Interval Estimation

An interval estimate provides a range of values within which the unknown population parameter is expected to lie, with a specified level of confidence.

For example:

Instead of saying that the average marks are exactly 72, we may estimate that the population average lies between 69 and 75.

This range is called a **confidence interval**.

---

# Part B: Confidence Intervals

## 5. What Is a Confidence Interval?

A confidence interval is a range of values calculated from sample data to estimate an unknown population parameter.

It provides information about the uncertainty associated with an estimate.

For example:

A university surveys 100 students and estimates their average monthly expenditure as Rs. 12,000.

A confidence interval might be:

Rs. 11,000 to Rs. 13,000.

This means that the sample data support a range of plausible values for the population average.

### 5.1 Confidence Level

A confidence level tells us how reliable the interval estimation procedure is over repeated sampling.

Common confidence levels include:

| Confidence Level | Meaning |
|---|---|
| 90% | 90% confidence level |
| 95% | 95% confidence level |
| 99% | 99% confidence level |

The 95% confidence level is commonly used in statistical research.

A correct interpretation is:

If we repeatedly collected samples and constructed confidence intervals using the same method, approximately 95% of those intervals would contain the true population parameter.

**Important:** A 95% confidence interval does not mean that there is a 95% probability that the fixed population mean lies inside the particular interval we have already calculated.

### 5.2 Confidence Interval for a Population Mean

When the population standard deviation is known, a confidence interval for the population mean can be calculated using:

$$
\bar{x} \pm z_{\alpha/2}\left(\frac{\sigma}{\sqrt{n}}\right)
$$

Where:

- x̄ = Sample mean.
- z = Critical z-value.
- σ = Population standard deviation.
- n = Sample size.
- √n = Square root of the sample size.

The expression:

$$
\frac{\sigma}{\sqrt{n}}
$$

is called the **standard error of the mean** when the population standard deviation is known.

For a 95% confidence interval, the critical z-value is approximately 1.96.

For a 90% confidence interval, it is approximately 1.645.

For a 99% confidence interval, it is approximately 2.576.

### 5.3 A Simple Example

Suppose:

- Sample mean = 70
- Population standard deviation = 10
- Sample size = 100
- Confidence level = 95%

We want to estimate the population mean.

The formula is:

$$
\bar{x} \pm z_{\alpha/2}\left(\frac{\sigma}{\sqrt{n}}\right)
$$

Substitute the values:

$$
70 \pm 1.96\left(\frac{10}{\sqrt{100}}\right)
$$

Since:

$$
\sqrt{100} = 10
$$

Therefore:

$$
70 \pm 1.96(1)
$$

$$
70 \pm 1.96
$$

The lower limit is:

$$
70 - 1.96 = 68.04
$$

The upper limit is:

$$
70 + 1.96 = 71.96
$$

Therefore, the 95% confidence interval is:

$$
\boxed{(68.04,\ 71.96)}
$$

**Interpretation:** Using this method, we estimate the population mean to be between 68.04 and 71.96, with a 95% confidence level.

### 5.4 What Happens When the Confidence Level Changes?

Consider the following general observations:

- Higher confidence requires a wider interval.
- Lower confidence produces a narrower interval.
- Larger sample sizes generally produce narrower intervals.
- More variability in the data generally produces wider intervals.

For example, a 99% confidence interval will generally be wider than a 95% confidence interval calculated from the same sample.

This happens because we need a wider range to achieve a higher confidence level.

---

# Part C: Hypothesis Testing

## 6. What Is Hypothesis Testing?

Hypothesis testing is a statistical method used to evaluate a claim about a population using sample data.

In simple words, it helps us decide whether the evidence from a sample supports or contradicts a particular claim.

Consider these examples:

- Does a new teaching method improve examination results?
- Does a new medicine reduce recovery time?
- Is the average monthly expenditure of students Rs. 15,000?
- Does a new computer system reduce processing time?

We use hypothesis testing to examine such questions systematically.

## 7. Null and Alternative Hypotheses

Hypothesis testing involves two competing statements.

### 7.1 Null Hypothesis (H₀)

The null hypothesis represents the initial assumption or claim being tested.

It commonly states that:

- There is no significant difference.
- There is no significant effect.
- There is no change.
- A population parameter equals a specified value.

Example:

A university claims that the average examination mark is 60.

The null hypothesis is:

$$
H_0: \mu = 60
$$

### 7.2 Alternative Hypothesis (H₁)

The alternative hypothesis represents the possibility that the null hypothesis is not correct.

For example:

$$
H_1: \mu \neq 60
$$

This means that the average examination mark is different from 60.

### 7.3 Types of Alternative Hypotheses

There are three common forms.

**Two-tailed test:**

We want to determine whether the population mean is different from a specified value.

$$
H_1: \mu \neq 60
$$

**Right-tailed test:**

We want to determine whether the population mean is greater than a specified value.

$$
H_1: \mu > 60
$$

**Left-tailed test:**

We want to determine whether the population mean is less than a specified value.

$$
H_1: \mu < 60
$$

The choice depends on the research question and must be made before examining the test result.

## 8. Significance Level

The significance level is the threshold used to decide whether the sample provides sufficient evidence against the null hypothesis.

It is represented by:

$$
\alpha
$$

Common significance levels are:

- 0.10 (10%)
- 0.05 (5%)
- 0.01 (1%)

A significance level of 0.05 is commonly used.

It means that we accept a 5% risk of rejecting a true null hypothesis when using this testing procedure.

This error is called a **Type I Error**.

### Type I and Type II Errors

| Error | Meaning |
|---|---|
| Type I Error | Rejecting a true null hypothesis. |
| Type II Error | Failing to reject a false null hypothesis. |

Example:

Suppose a university is testing whether a new teaching method improves student performance.

- Type I Error: Concluding that the method improves performance when it actually does not.
- Type II Error: Failing to detect a genuine improvement.

These errors remind us that statistical decisions involve uncertainty.

## 9. The p-value

The p-value is an important concept in hypothesis testing.

It measures how unusual the observed sample result, or a more extreme result, would be if the null hypothesis were true.

In simple terms, a small p-value indicates that the observed data would be relatively unlikely under the null hypothesis.

A common decision rule is:

- If p-value ≤ 0.05, reject the null hypothesis.
- If p-value > 0.05, fail to reject the null hypothesis.

Example:

Suppose a statistical test produces:

$$
p = 0.03
$$

Using a significance level of:

$$
\alpha = 0.05
$$

Since:

$$
0.03 < 0.05
$$

We reject the null hypothesis.

The result is statistically significant at the 5% level.

**Important:** A p-value is not the probability that the null hypothesis is true. Also, statistical significance does not necessarily mean that an effect is large or practically important.

---

# Part D: z-Test and t-Test

## 10. What Is a z-Test?

A z-test is a statistical test commonly used to examine a population mean when the population standard deviation is known and the sampling conditions are appropriate.

It compares the sample mean with a hypothesized population mean.

The z-test statistic for a population mean is:

$$
z = \frac{\bar{x} - \mu_0}{\sigma/\sqrt{n}}
$$

Where:

- x̄ = Sample mean.
- μ₀ = Mean stated in the null hypothesis.
- σ = Known population standard deviation.
- n = Sample size.

The calculated z-value indicates how far the sample mean is from the hypothesized population mean, measured in standard errors.

### 10.1 Example of a z-Test

Suppose a university claims that the average examination mark is 60.

A sample of 100 students produces:

- Sample mean = 63
- Population standard deviation = 10
- Sample size = 100

We want to test whether the population mean is different from 60.

**Step 1: State the hypotheses**

$$
H_0: \mu = 60
$$

$$
H_1: \mu \neq 60
$$

**Step 2: Identify the values**

$$
\bar{x} = 63
$$

$$
\mu_0 = 60
$$

$$
\sigma = 10
$$

$$
n = 100
$$

**Step 3: Apply the z-test formula**

$$
z = \frac{\bar{x} - \mu_0}{\sigma/\sqrt{n}}
$$

Substitute the values:

$$
z = \frac{63 - 60}{10/\sqrt{100}}
$$

Since:

$$
\sqrt{100} = 10
$$

We get:

$$
z = \frac{3}{10/10}
$$

$$
z = \frac{3}{1}
$$

$$
\boxed{z = 3}
$$

**Step 4: Interpret the result**

For a two-tailed test at the 5% significance level, the critical z-values are approximately:

$$
-1.96 \quad \text{and} \quad +1.96
$$

Our calculated value is:

$$
z = 3
$$

Since 3 is greater than 1.96, we reject the null hypothesis.

**Conclusion:** The sample provides statistically significant evidence that the population mean is different from 60 at the 5% significance level.

---

## 11. What Is a t-Test?

A t-test is another statistical method used to examine a population mean.

It is particularly useful when:

- The population standard deviation is unknown.
- We estimate variability using the sample standard deviation.
- The data and sampling conditions are suitable for the test.

The t-test is especially useful for smaller samples when the population is approximately normally distributed.

The t-test statistic for a one-sample mean is:

$$
t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}
$$

Where:

- x̄ = Sample mean.
- μ₀ = Mean stated in the null hypothesis.
- s = Sample standard deviation.
- n = Sample size.

Notice that the t-test uses the sample standard deviation (s), while the z-test uses the known population standard deviation (σ).

### 11.1 Example of a t-Test

Suppose a researcher wants to test whether the average study time of students is 4 hours per day.

A sample of 16 students produces:

- Sample mean = 5 hours.
- Sample standard deviation = 2 hours.
- Sample size = 16.

We want to determine whether the population average study time is different from 4 hours.

**Step 1: State the hypotheses**

$$
H_0: \mu = 4
$$

$$
H_1: \mu \neq 4
$$

**Step 2: Identify the values**

$$
\bar{x} = 5
$$

$$
\mu_0 = 4
$$

$$
s = 2
$$

$$
n = 16
$$

**Step 3: Apply the t-test formula**

$$
t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}
$$

Substitute the values:

$$
t = \frac{5 - 4}{2/\sqrt{16}}
$$

Since:

$$
\sqrt{16} = 4
$$

We get:

$$
t = \frac{1}{2/4}
$$

$$
t = \frac{1}{0.5}
$$

$$
\boxed{t = 2}
$$

**Step 4: Understand degrees of freedom**

For a one-sample t-test, degrees of freedom are calculated as:

$$
df = n - 1
$$

Therefore:

$$
df = 16 - 1 = 15
$$

The critical t-value depends on the degrees of freedom and significance level.

For a two-tailed test at the 5% significance level with 15 degrees of freedom, the critical values are approximately:

$$
-2.131 \quad \text{and} \quad +2.131
$$

Our calculated t-value is 2.

Since 2 lies between -2.131 and +2.131, we fail to reject the null hypothesis.

**Conclusion:** The sample does not provide sufficient evidence at the 5% significance level that the population mean study time differs from 4 hours.

This does not prove that the population mean is exactly 4 hours. It only means that the evidence is insufficient to reject the null hypothesis.

---

## 12. Difference Between z-Test and t-Test

Both tests are used to investigate claims about population means, but they differ in their assumptions and applications.

| z-Test | t-Test |
|---|---|
| Uses the population standard deviation (σ). | Uses the sample standard deviation (s). |
| Commonly used when population standard deviation is known. | Commonly used when population standard deviation is unknown. |
| Uses the standard normal distribution. | Uses the t-distribution. |
| Does not require estimating degrees of freedom for the standard one-sample z-test. | Uses degrees of freedom. |
| Often used in large-sample settings or when σ is known. | Particularly useful for smaller samples when σ is unknown and normality assumptions are reasonable. |

### Why Are There Two Tests?

When the population standard deviation is unknown, we estimate it using the sample standard deviation.

This introduces additional uncertainty.

The t-distribution accounts for this extra uncertainty. It has heavier tails than the standard normal distribution, especially with small samples.

As the sample size increases, the t-distribution approaches the standard normal distribution.

**A useful rule for introductory learning:**

- Known population standard deviation: consider a z-test.
- Unknown population standard deviation: consider a t-test.

The actual choice also depends on the sampling design, distribution of the data, and other test assumptions.

---

# Part E: Statistical Inference and Decision-Making

## 13. What Is Statistical Inference?

Statistical inference is the process of using sample information to draw conclusions about a population.

It includes:

1. Estimation
2. Confidence intervals
3. Hypothesis testing

These techniques help us make decisions when complete population information is unavailable.

### 13.1 Estimation vs Hypothesis Testing

| Estimation | Hypothesis Testing |
|---|---|
| Estimates an unknown population value. | Tests a claim about a population. |
| Produces a point estimate or interval. | Produces a statistical decision. |
| Example: Estimate average student marks. | Example: Test whether average marks equal 60. |

### 13.2 A Practical Example

Suppose a university introduces a new teaching method.

The university wants to know whether the new method improves examination performance.

A possible research procedure is:

**Step 1: Collect Data**

Select a sample of students taught using the new method.

**Step 2: Calculate an Estimate**

Calculate their average examination marks.

**Step 3: Construct a Confidence Interval**

Estimate a range for the population's average examination marks.

**Step 4: Form Hypotheses**

For example:

$$
H_0: \mu_{\text{new}} = \mu_{\text{old}}
$$

$$
H_1: \mu_{\text{new}} > \mu_{\text{old}}
$$

**Step 5: Conduct a Statistical Test**

Select an appropriate test based on the study design and available information.

**Step 6: Interpret the Result**

Determine whether the sample provides sufficient evidence that the new method improves performance.

This is an example of using statistical inference to support an educational decision.

---

# Part F: Practical Exercises

## 14. Exercise 1: Population and Sample

A university has 5,000 students. A researcher selects 200 students to study their average daily study time.

Answer:

1. Identify the population.
2. Identify the sample.
3. Why might the researcher select a sample instead of studying all students?
4. What problems might occur if the sample includes only students from one department?

## 15. Exercise 2: Point and Interval Estimation

A sample of 50 students has an average examination mark of 65.

Answer:

1. What is the point estimate of the population mean?
2. Is 65 guaranteed to be the actual population mean?
3. What is the difference between point estimation and interval estimation?
4. Why might an interval estimate be more informative?

## 16. Exercise 3: Confidence Interval Interpretation

A researcher calculates a 95% confidence interval for average monthly student expenditure:

Rs. 10,000 to Rs. 14,000.

Answer:

1. What is the estimated interval?
2. What does the 95% confidence level mean?
3. Would a 99% confidence interval generally be wider or narrower?
4. What happens to the interval width when the sample size increases, assuming other factors remain unchanged?

## 17. Exercise 4: Hypothesis Testing

A university claims that the average examination mark is 60.

Write the null and alternative hypotheses for each situation:

1. The researcher wants to test whether the average mark is different from 60.
2. The researcher wants to test whether the average mark is greater than 60.
3. The researcher wants to test whether the average mark is less than 60.

## 18. Exercise 5: Interpret p-values

A statistical test produces the following results:

| Case | p-value | Significance Level |
|---|---:|---:|
| A | 0.02 | 0.05 |
| B | 0.08 | 0.05 |
| C | 0.001 | 0.01 |
| D | 0.04 | 0.01 |

For each case, decide whether to reject or fail to reject the null hypothesis.

## 19. Exercise 6: Understand z-Test and t-Test

Answer the following:

1. What is a z-test?
2. What is a t-test?
3. Which test commonly uses the population standard deviation?
4. Which test uses the sample standard deviation?
5. Why does the t-distribution have heavier tails than the standard normal distribution, particularly for small samples?
6. What are degrees of freedom?

## 20. Exercise 7: Basic Calculations

### Question A: z-Test

Given:

- Sample mean = 52
- Hypothesized population mean = 50
- Population standard deviation = 8
- Sample size = 64

Calculate the z-test statistic using:

$$
z = \frac{\bar{x} - \mu_0}{\sigma/\sqrt{n}}
$$

### Question B: t-Test

Given:

- Sample mean = 45
- Hypothesized population mean = 40
- Sample standard deviation = 10
- Sample size = 25

Calculate the t-test statistic using:

$$
t = \frac{\bar{x} - \mu_0}{s/\sqrt{n}}
$$

Also calculate the degrees of freedom.

---

# 21. Key Takeaways

1. A population is the complete group being studied.
2. A sample is a smaller group selected from the population.
3. Estimation uses sample information to approximate population parameters.
4. Point estimation gives a single estimated value.
5. Interval estimation provides a range of plausible values.
6. A confidence interval describes the reliability of an estimation procedure.
7. Hypothesis testing evaluates a claim about a population using sample data.
8. The null hypothesis represents the initial claim being tested.
9. The alternative hypothesis represents the competing claim.
10. A p-value helps us evaluate the evidence against the null hypothesis.
11. A z-test commonly uses a known population standard deviation.
12. A t-test commonly uses a sample standard deviation when the population standard deviation is unknown.
13. Statistical inference helps us make evidence-based decisions.

---

# 22. Final Thought

Imagine that a university wants to know whether a new teaching method improves student performance.

It is usually impractical to test every student in the university.

Instead, the university can:

- Select a representative sample.
- Calculate the average marks.
- Estimate the population average.
- Construct a confidence interval.
- Conduct a hypothesis test.
- Interpret the evidence and make a decision.

This is the fundamental purpose of statistical inference:

**We use information from a sample to make informed conclusions about a larger population, while recognizing that every estimate and decision involves some uncertainty.**
