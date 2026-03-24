# Quantitative Data Analysis

## Selecting Statistical Procedures

Your choice of statistical test depends on three factors (Field, 2018; Tabachnick & Fidell, 2013):

1. **Your research question**: Are you describing, comparing, predicting, or examining relationships?
2. **Your data type**: Continuous (interval/ratio) or categorical (nominal/ordinal)?
3. **Assumptions**: Does your data meet the requirements of the test?

---

## Common Statistical Procedures for Dissertation Research

```{list-table} Matching Research Questions to Statistical Tests
:header-rows: 1
:widths: 25 15 15 20

* - Research Question
  - IV Type
  - DV Type
  - Procedure
* - Difference between 2 groups
  - Categorical (2 levels)
  - Continuous
  - Independent samples t-test
* - Difference among 3+ groups
  - Categorical (3+ levels)
  - Continuous
  - One-way ANOVA
* - Relationship between 2 variables
  - Continuous
  - Continuous
  - Pearson correlation
* - Prediction from multiple variables
  - Multiple continuous/categorical
  - Continuous
  - Multiple regression
* - Group differences on multiple DVs
  - Categorical
  - Multiple continuous
  - MANOVA
* - Category associations
  - Categorical
  - Categorical
  - Chi-square test
* - Prediction of group membership
  - Multiple continuous/categorical
  - Categorical
  - Logistic regression
```

```{tip}
Spector (2013, Ch. 9) provides additional guidance on selecting statistical procedures within the context of social science research design, including considerations for nested data and repeated measures.
```

---

## Assumption Checking

Before running any parametric test, you must verify that your data meet the test's assumptions. Tabachnick and Fidell (2013, Ch. 4) provide the definitive treatment of this topic.

### Key Assumptions for Parametric Tests

**Normality**
: The dependent variable should be approximately normally distributed within each group. Assessed through Shapiro-Wilk test, Q-Q plots, and skewness/kurtosis values. Minor violations are tolerable with large samples (central limit theorem), but severe violations require transformation or non-parametric alternatives.

**Homogeneity of variance**
: Variance of the dependent variable should be similar across groups. Assessed through Levene's test. Violations can be addressed with robust alternatives (Welch's t-test, Brown-Forsythe ANOVA).

**Linearity**
: For correlation and regression, the relationship between variables should be approximately linear. Assessed through scatterplot inspection and residual plots.

**Independence**
: Observations should be independent of each other. This is primarily a *design* assumption — ensured through random sampling and proper research procedures.

**Absence of multicollinearity** (for regression)
: Predictor variables should not be too highly correlated with each other. Assessed through Variance Inflation Factor (VIF < 10) and tolerance statistics.

```{warning}
Never skip assumption checking. Reporting statistical results from tests whose assumptions are violated can lead to incorrect conclusions — Type I or Type II errors that undermine your entire study. Your methodology chapter should describe how you will check assumptions *before* running your primary analyses.
```

See the {doc}`notebook-analysis-tools` for an interactive assumption-checking dashboard.

---

## Effect Sizes and Practical Significance

Statistical significance (p < .05) tells you whether an effect is likely *real*; effect size tells you whether it *matters*. APA 7th edition requires reporting effect sizes alongside p-values.

### Cohen's (1992) Conventional Benchmarks

| Measure | Context | Small | Medium | Large |
|---------|---------|-------|--------|-------|
| *d* | Mean differences (t-tests) | 0.20 | 0.50 | 0.80 |
| *r* | Correlations | 0.10 | 0.30 | 0.50 |
| η² | Variance explained (ANOVA) | 0.01 | 0.06 | 0.14 |
| *f* | ANOVA effect size | 0.10 | 0.25 | 0.40 |

```{important}
Cohen himself cautioned that these are *conventions*, not absolute standards. A "small" effect size can be practically significant in some contexts (e.g., a medical intervention), and a "large" effect can be trivial in others. Always interpret effect sizes in the context of your research domain.
```

---

## Variable Operationalization

Your methodology chapter must specify how each variable in your study will be measured:

1. **Conceptual definition**: What does the variable mean theoretically?
2. **Operational definition**: How will you measure it? What specific instrument, item, or procedure?
3. **Level of measurement**: Nominal, ordinal, interval, or ratio?
4. **Role in analysis**: Independent variable, dependent variable, covariate, moderator, mediator?

```{admonition} Example
:class: note
**Variable**: Information Literacy Self-Efficacy

- *Conceptual definition*: An individual's confidence in their ability to find, evaluate, and use information effectively
- *Operational definition*: Score on the Information Literacy Self-Efficacy Scale (Kurbanoglu, Akkoyunlu, & Umay, 2006), a 28-item Likert-type instrument
- *Level of measurement*: Interval (composite score from 28–196)
- *Role*: Dependent variable in RQ1; independent variable in RQ2
```

---

## Reporting Quantitative Results

Your analysis plan should specify the format for reporting results, following APA 7th edition conventions:

- Report exact p-values (not just p < .05 or p > .05)
- Include effect sizes and confidence intervals
- Present descriptive statistics (means, standard deviations) alongside inferential statistics
- Use tables and figures to present complex results clearly
- Describe the practical significance, not just statistical significance

---

## ✏️ Exercise: Draft Your Quantitative Analysis Plan

Write a 2–3 page analysis plan section that:

1. **Lists each research question or hypothesis** with the corresponding statistical test
2. **Operationalizes all variables**: Conceptual definition, operational definition, measurement level, role
3. **Specifies assumption-checking procedures**: What will you check, how, and what will you do if assumptions are violated?
4. **Describes your analytic software**: SPSS, R, Python, etc.
5. **Reports your power analysis**: Test, effect size, alpha, power, required N (connect to your sampling plan in Block 1)
6. **States your approach to missing data**: Listwise deletion, pairwise deletion, imputation?
