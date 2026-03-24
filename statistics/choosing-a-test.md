# Choosing a Statistical Test

This chapter is a practical decision guide. Given your research question and data types, it helps you identify the appropriate statistical procedure. Bookmark this page:  you'll come back to it.

---

## The Decision Framework

Choosing a test requires answering three questions:

1. **What is your research question asking?** (difference, relationship, or prediction)
2. **What type of data do you have?** (the measurement level of your IV and DV)
3. **How many groups or variables are involved?**

---

## Tests for Differences Between Groups

*"Is there a difference between these groups?"*

```{list-table}
:header-rows: 1

* - Situation
  - Parametric Test
  - Nonparametric Alternative
  - When to Use Nonparametric
* - 2 independent groups, continuous DV
  - **Independent samples t-test**
  - Mann-Whitney U test
  - Ordinal DV or non-normal distribution
* - 2 related groups (pre/post or matched)
  - **Paired samples t-test**
  - Wilcoxon signed-rank test
  - Ordinal DV or non-normal differences
* - 3+ independent groups, continuous DV
  - **One-way ANOVA**
  - Kruskal-Wallis H test
  - Ordinal DV or non-normal distribution
* - 3+ related groups (repeated measures)
  - **Repeated measures ANOVA**
  - Friedman test
  - Ordinal DV or violated sphericity
* - 2+ groups, 2+ continuous DVs simultaneously
  - **MANOVA**
  - (no simple equivalent)
  - When you have multiple related outcomes
* - 2 categorical variables
  - **Chi-square test of independence**
  - Fisher's exact test
  - When expected cell counts are < 5
```

### When to Use Each

**t-test**: You have one IV with two groups and one continuous DV. Example: "Do library users who receive instruction score higher on an information literacy test than those who don't?"

**ANOVA**: You have one IV with three or more groups and one continuous DV. Example: "Do satisfaction scores differ among users of academic, public, and special libraries?" If ANOVA is significant, follow up with *post-hoc tests* (Tukey, Bonferroni) to determine which specific groups differ.

**Chi-square**: Both your variables are categorical. Example: "Is there an association between library type and whether users prefer print or digital resources?"

---

## Tests for Relationships Between Variables

*"Is there a relationship between these variables?"*

```{list-table}
:header-rows: 1

* - Situation
  - Test
  - Output
* - 2 continuous variables
  - **Pearson correlation (*r*)**
  - Strength and direction of linear relationship
* - 2 ordinal variables (or non-normal continuous)
  - **Spearman correlation (*rₛ*)**
  - Rank-order relationship
* - 1 continuous + 1 dichotomous (binary)
  - **Point-biserial correlation**
  - Strength of association
* - 2 nominal variables
  - **Cramér's V** (from chi-square)
  - Strength of association between categories
```

```{important}
**Correlation does not imply causation.** A significant correlation between two variables means they are *associated*:  they tend to move together. It does not tell you that one causes the other. There may be a third variable causing both, or the causal direction may be reversed, or the relationship may be coincidental.
```

---

## Tests for Prediction

*"Can I predict this outcome from these predictors?"*

```{list-table}
:header-rows: 1

* - Situation
  - Test
  - What It Does
* - Predict a continuous DV from one or more IVs
  - **Multiple linear regression**
  - Estimates how much each IV contributes to predicting the DV; produces R² (total variance explained)
* - Predict a categorical DV (yes/no) from one or more IVs
  - **Logistic regression**
  - Estimates the probability of group membership; produces odds ratios
* - Predict a DV while controlling for covariates
  - **Hierarchical regression**
  - Enter predictors in theoretically meaningful blocks to see how much each block adds
* - Test a complex theoretical model with multiple relationships
  - **Structural equation modeling (SEM)**
  - Tests an entire network of relationships simultaneously; see [Advanced Methods](advanced-methods.md)
```

---

## Quick-Reference Decision Tree

Ask yourself these questions in order:

**1. What does your research question ask?**
- Difference → go to differences section
- Relationship → go to relationships section
- Prediction → go to prediction section

**2. What type is your dependent variable?**
- Continuous (interval/ratio) → parametric tests available
- Categorical (nominal/ordinal) → nonparametric or chi-square

**3. How many groups or predictors?**
- 2 groups → t-test
- 3+ groups → ANOVA
- 1 predictor → simple regression or correlation
- 2+ predictors → multiple regression

**4. Are your data independent or related?**
- Independent groups (different people) → independent samples tests
- Related groups (same people measured twice, or matched pairs) → paired/repeated measures tests

---

## Assumption Checking: Before You Run Any Test

Every parametric test has assumptions that must be checked (Tabachnick & Fidell, 2013). Running a test when assumptions are violated can produce misleading results.

| Assumption | What It Means | How to Check | What to Do If Violated |
|------------|---------------|--------------|----------------------|
| **Normality** | DV is approximately normally distributed | Shapiro-Wilk test, Q-Q plot, histogram | Use nonparametric alternative or transform data |
| **Homogeneity of variance** | Variance is similar across groups | Levene's test | Use Welch's t-test or Brown-Forsythe ANOVA |
| **Independence** | Observations are not related to each other | Research design (not a statistical test) | Use repeated measures or multilevel models |
| **Linearity** | Relationship between variables is linear | Scatterplot, residual plot | Consider polynomial terms or nonlinear models |
| **No multicollinearity** | Predictors are not too highly correlated | VIF (Variance Inflation Factor) < 10 | Remove or combine redundant predictors |

```{admonition} Key Reading
:class: seealso
See the [Analysis Tools notebook](../block3/notebook-analysis-tools.ipynb) for an interactive assumption-checking dashboard you can use with your own data.
```
