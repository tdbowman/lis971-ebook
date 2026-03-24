# Foundations: Variables, Measurement, and Distributions

## What Is a Variable?

A variable is any characteristic that can take on different values across people, places, or time. In research, everything you measure or observe is a variable.

**Examples in LIS research:**
- Number of library visits per month
- Satisfaction with reference services (on a 1–5 scale)
- Type of library (academic, public, special, school)
- Whether a user found the information they needed (yes/no)

### Types of Variables by Role

When you design a study, each variable plays a specific role:

**Independent variable (IV)**
: The variable you believe *causes* or *predicts* something. In an experiment, it's what you manipulate. In a survey, it's what you think explains differences in outcomes.

**Dependent variable (DV)**
: The variable you are trying to *explain* or *predict*. It's the outcome the thing that changes (or doesn't) depending on the IV.

**Control variable (covariate)**
: A variable you account for so it doesn't confuse your results. For example, controlling for age when studying the relationship between technology experience and information literacy.

**Moderator**
: A variable that changes the *strength or direction* of the relationship between the IV and DV. For example, digital literacy might moderate the relationship between database design and search success.

**Mediator**
: A variable that *explains the mechanism* through which the IV affects the DV. For example, self-efficacy might mediate the relationship between a training program and research performance.

---

## Levels of Measurement

How you measure a variable determines which statistics you can use. This is one of the most practically important concepts in the entire section.

```{list-table} The Four Levels of Measurement
:header-rows: 1

* - Level
  - What It Means
  - Examples
  - What You Can Do
* - **Nominal**
  - Categories with no order
  - Gender, library type, yes/no, department
  - Count, mode, chi-square
* - **Ordinal**
  - Categories with a meaningful order, but unequal gaps between them
  - Satisfaction ratings (low/medium/high), education level, Likert items
  - Median, percentiles, rank-order tests
* - **Interval**
  - Equal gaps between values, but no true zero
  - Temperature (°F), standardized test scores, Likert scale composites (debated)
  - Mean, standard deviation, t-tests, ANOVA, correlation
* - **Ratio**
  - Equal gaps AND a true zero (zero means "none")
  - Number of visits, income, time spent, word count
  - All of the above plus ratios ("twice as many")
```

```{important}
**The practical takeaway:** Nominal and ordinal variables require *nonparametric* tests (chi-square, Mann-Whitney). Interval and ratio variables can use *parametric* tests (t-test, ANOVA, regression) assuming other conditions are met. Getting this wrong is one of the most common statistical errors in dissertation research.
```

### The Likert Scale Debate

A single Likert item ("Strongly Disagree" to "Strongly Agree") is technically ordinal the distance between "Agree" and "Strongly Agree" isn't necessarily the same as between "Disagree" and "Neutral." However, when you create a *composite score* by averaging multiple Likert items measuring the same construct, many researchers treat the result as interval data. This is common and generally accepted practice, but you should acknowledge the assumption in your methodology chapter.

---

## Distributions: What Your Data Look Like

A distribution describes how values are spread across your variable. Understanding distributions helps you choose the right statistical test and interpret your results.

### The Normal Distribution

The normal distribution (the "bell curve") is the foundation of most parametric statistics. It has these properties:

- Symmetric around the mean
- Mean = Median = Mode
- About 68% of scores fall within 1 standard deviation of the mean
- About 95% fall within 2 standard deviations
- About 99.7% fall within 3 standard deviations

Most parametric tests (t-tests, ANOVA, regression) *assume* your data are approximately normally distributed. When they're not, you may need to transform your data or use nonparametric alternatives.

### Skewness and Kurtosis

**Skewness** describes whether the distribution leans to one side:
- *Positive skew* (right-skewed): Long tail to the right. Example: income data most people cluster at lower values, with a few very high earners pulling the tail right.
- *Negative skew* (left-skewed): Long tail to the left. Example: exam scores in an easy course most people score high.

**Kurtosis** describes the "peakedness" of the distribution:
- *Leptokurtic* (positive kurtosis): Tall and narrow with heavy tails more extreme values than a normal distribution
- *Platykurtic* (negative kurtosis): Flat and wide fewer extreme values

```{tip}
As a rule of thumb, skewness and kurtosis values between -1 and +1 suggest approximate normality. Values beyond ±2 indicate a distribution that may cause problems for parametric tests. See the assumption-checking notebook in Block 3 for tools to assess this visually.
```

---

## Populations and Samples

**Population**: Everyone (or everything) you want to draw conclusions about all public librarians in Illinois, all first-generation doctoral students, all tweets containing a particular hashtag.

**Sample**: The subset you actually study. You collect data from a sample and use statistics to make *inferences* about the population.

**Sampling error**: The inevitable difference between your sample statistics and the true population values. Larger samples produce less sampling error.

**Standard error**: A measure of how much your sample statistic (like the mean) would vary if you drew many different samples from the same population. Smaller standard errors mean more precise estimates.

---

## Key Vocabulary Summary

Here are the terms you'll see repeatedly in methodology chapters and statistical output:

| Term | Plain-Language Definition |
|------|--------------------------|
| **Variable** | Anything you measure that can differ across cases |
| **Parameter** | A characteristic of the *population* (usually unknown) |
| **Statistic** | A characteristic of the *sample* (what you calculate) |
| **Variance** | How spread out the scores are from the mean |
| **Standard deviation** | The average distance of scores from the mean (square root of variance) |
| **Normal distribution** | The symmetric bell curve that many statistical tests assume |
| **Degrees of freedom (df)** | The number of values free to vary in a calculation affects critical values for tests |
| **Statistical significance** | The probability that your result occurred by chance alone (typically p < .05) |
| **Effect size** | How large and meaningful the result is, independent of sample size |
