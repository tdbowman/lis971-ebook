# Inferential Statistics: Drawing Conclusions from Data

Descriptive statistics summarize *your sample*. Inferential statistics help you draw conclusions about the *population* your sample came from. This is the heart of quantitative reasoning: using limited data to make general claims.

---

## The Logic of Hypothesis Testing

Hypothesis testing follows a consistent logic, regardless of which specific test you use:

**Step 1 State two competing hypotheses:**
- The *null hypothesis* (H₀): There is no effect, no difference, no relationship. This is the default assumption.
- The *alternative hypothesis* (H₁ or Hₐ): There *is* an effect, difference, or relationship. This is what you're trying to find evidence for.

**Step 2 Collect data and calculate a test statistic:**
The test statistic (like *t*, *F*, or χ²) quantifies how far your sample result is from what the null hypothesis predicts.

**Step 3 Determine the probability (p-value):**
The p-value answers: *If the null hypothesis were true, how likely is it that I would get a result at least this extreme?*

**Step 4 Make a decision:**
- If p < .05 (conventional threshold): Reject H₀. The result is "statistically significant."
- If p ≥ .05: Fail to reject H₀. You did not find sufficient evidence to support your alternative hypothesis.

```{important}
**"Fail to reject" is not the same as "prove the null is true."** A non-significant result means you didn't find enough evidence not that there is definitely no effect. The effect might exist but be too small for your sample size to detect (a problem of *statistical power*).
```

---

## Understanding the p-Value

The p-value is the single most misunderstood concept in statistics. Here's what it means and what it does not mean:

**What the p-value IS:**
The probability of obtaining results at least as extreme as yours, *assuming the null hypothesis is true*.

**What the p-value is NOT:**
- The probability that the null hypothesis is true
- The probability that your results are due to chance
- A measure of how important or meaningful the effect is
- A guarantee that the effect is real

**The .05 threshold** is a convention, not a law of nature. Fisher originally proposed it as a reasonable benchmark, and Cohen (1992) and others have noted that it is arbitrary. Some fields use .01 or .001 for greater stringency. APA 7th edition recommends reporting *exact* p-values (e.g., p = .032) rather than just p < .05.

---

## Two Types of Errors

Every decision in hypothesis testing carries a risk of error:

| | You Reject H₀ | You Fail to Reject H₀ |
|---|---|---|
| **H₀ is actually true** | **Type I Error** (false positive) you think there's an effect when there isn't | Correct decision |
| **H₀ is actually false** | Correct decision | **Type II Error** (false negative) you miss a real effect |

**Alpha (α)**: The probability of a Type I error. By convention, α = .05 means you accept a 5% chance of a false positive.

**Beta (β)**: The probability of a Type II error. By convention, β = .20 means you accept a 20% chance of missing a real effect.

**Power (1 - β)**: The probability of correctly detecting a real effect. Convention: power = .80 (80% chance of finding an effect that actually exists).

---

## Effect Sizes: How Big Is the Effect?

Statistical significance tells you whether an effect is likely *real*; effect size tells you whether it *matters*. A tiny, practically meaningless effect can be "statistically significant" with a large enough sample. APA 7th edition *requires* reporting effect sizes.

### Cohen's d (for differences between means)

How many standard deviations apart are the two group means?

| Value | Interpretation |
|-------|---------------|
| 0.20 | Small effect |
| 0.50 | Medium effect |
| 0.80 | Large effect |

**Example:** "The training group scored significantly higher than the control group, *t*(48) = 2.85, *p* = .006, *d* = 0.72" a medium-to-large effect.

### Pearson's r (for relationships between variables)

How strongly are two continuous variables related?

| Value | Interpretation |
|-------|---------------|
| .10 | Small / weak |
| .30 | Medium / moderate |
| .50 | Large / strong |

**Example:** "There was a moderate positive correlation between information literacy scores and GPA, *r*(98) = .34, *p* < .001."

### η² (eta-squared) and partial η² (for ANOVA)

What proportion of the total variance in the DV is explained by the IV?

| Value | Interpretation |
|-------|---------------|
| .01 | Small |
| .06 | Medium |
| .14 | Large |

### R² (for regression)

What proportion of variance in the DV is explained by all the predictors combined?

**Example:** "The regression model explained 42% of the variance in user satisfaction, *R²* = .42, *F*(3, 96) = 23.15, *p* < .001."

```{warning}
Cohen (1992) himself cautioned that these benchmarks are *conventions*, not absolute standards. A "small" effect can be practically important in some contexts (medical treatments that save lives), and a "large" effect can be trivial in others. Always interpret effect sizes within the context of your research domain.
```

---

## Confidence Intervals

A confidence interval provides a range of plausible values for the true population parameter, based on your sample data.

**Example:** "The mean satisfaction score was 3.82, 95% CI [3.61, 4.03]."

This means: if we repeated this study many times, 95% of the resulting confidence intervals would contain the true population mean.

**Practical interpretation:** You can be reasonably confident the true mean is somewhere between 3.61 and 4.03. A narrow interval suggests a precise estimate; a wide one suggests more uncertainty (usually due to a small sample or high variability).

```{tip}
Confidence intervals provide *more information* than p-values alone. They tell you not just whether the effect is significant, but how large or small the effect might plausibly be. APA 7th edition recommends reporting confidence intervals alongside significance tests.
```

---

## Statistical Power and Sample Size

Power is the probability that your study will detect a real effect if one exists. Low power means you might miss real effects a waste of time, effort, and participants' goodwill.

Power depends on four interconnected elements (Cohen, 1992):

1. **Effect size**: Larger effects are easier to detect
2. **Sample size**: More participants = more power
3. **Alpha level**: More stringent alpha (e.g., .01 vs .05) = less power
4. **Power itself**: Convention is .80 (80% chance of detecting a real effect)

If you know any three of these, you can calculate the fourth. The most common use is determining the *sample size* needed to detect an expected effect with adequate power.

```{admonition} Key Reading
:class: seealso
See the [Power Analysis notebook](../block1/notebook-power-analysis.ipynb) for an interactive calculator that computes required sample sizes for common tests.
```

---

## Putting It All Together: Reading a Statistical Result

When you see a result like this in a journal article:

> *"Participants in the instruction group scored significantly higher on the information literacy assessment (M = 82.3, SD = 11.4) than the control group (M = 74.1, SD = 12.8), t(78) = 3.02, p = .003, d = 0.68, 95% CI [2.82, 13.58]."*

Here's how to read each piece:

| Component | What It Tells You |
|-----------|-------------------|
| *M* = 82.3 and 74.1 | The average scores for each group |
| *SD* = 11.4 and 12.8 | How spread out scores are within each group |
| *t*(78) = 3.02 | The test statistic and degrees of freedom |
| *p* = .003 | The result is statistically significant (< .05) |
| *d* = 0.68 | A medium-to-large effect practically meaningful |
| 95% CI [2.82, 13.58] | The true difference is likely between about 3 and 14 points |
