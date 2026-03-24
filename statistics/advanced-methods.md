# Advanced Quantitative Methods

This chapter introduces statistical methods you may encounter in the research literature, need for your own dissertation, or hear about from committee members. Each entry provides a plain-language description, when to use it, and key terms you'll need to understand.

```{tip}
You don't need to master all of these. Focus on the methods relevant to your own study, but familiarize yourself with the others so you can read research that uses them and engage with committee feedback.
```

---

## Multiple Regression

**What it does:** Predicts a continuous outcome from two or more predictor variables simultaneously. Tells you how much each predictor contributes while controlling for the others.

**When to use it:** When you want to understand which variables predict an outcome and how much variance they explain together.

**Key concepts:**
- **R²** the proportion of variance in the DV explained by all predictors combined (e.g., R² = .35 means 35% of the variance is explained)
- **β (beta weights)** standardized regression coefficients showing the relative importance of each predictor
- **Adjusted R²** adjusts R² for the number of predictors (penalizes adding weak predictors)

**Example:** "Years of experience, education level, and technology training together predicted information literacy scores, *R²* = .41, *F*(3, 116) = 26.84, *p* < .001. Technology training was the strongest predictor (β = .38)."

---

## Hierarchical Regression

**What it does:** A variant of multiple regression where predictors are entered in theoretically meaningful *blocks* (steps). This lets you see how much each block adds to the prediction after controlling for what came before.

**When to use it:** When you have a theoretical reason for the order in which predictors should be considered. For example, entering demographic controls in Step 1, then your main predictors of interest in Step 2.

**Key concept:**
- **ΔR² (R-squared change)** how much additional variance each new block explains beyond the previous blocks

**Example:** "After controlling for age and education (Step 1, R² = .12), adding digital literacy and technology self-efficacy (Step 2) explained an additional 29% of variance in online search performance, ΔR² = .29, *p* < .001."

---

## Logistic Regression

**What it does:** Predicts a categorical outcome (usually yes/no) from one or more predictor variables. Instead of predicting a score, it predicts the *probability* of belonging to a category.

**When to use it:** When your DV is binary (e.g., completed a program or not; adopted a technology or not; found the information or not).

**Key concepts:**
- **Odds ratio (OR)** how much the odds of the outcome change for a one-unit increase in the predictor. OR = 1 means no effect; OR > 1 means increased odds; OR < 1 means decreased odds.
- **Classification accuracy** the percentage of cases the model correctly predicts

**Example:** "For each additional hour of training, the odds of successfully completing the database search task increased by 40%, OR = 1.40, 95% CI [1.12, 1.75], *p* = .003."

---

## Factor Analysis

**What it does:** Identifies clusters of variables that tend to move together, reducing many variables to a smaller number of underlying *factors* (latent constructs).

**Two types:**

**Exploratory Factor Analysis (EFA)**
: Used when you don't know what factors underlie your data. You let the data reveal the structure. Common in instrument development "I have 30 survey items; how do they group together?"

**Confirmatory Factor Analysis (CFA)**
: Used when you have a *hypothesized* factor structure (from theory or prior EFA) and want to test whether your data fit that structure. Common in instrument validation.

**Key concepts:**
- **Factor loadings** how strongly each variable relates to a factor (loadings above .40 are conventionally considered meaningful)
- **Eigenvalue** the amount of variance a factor explains (factors with eigenvalue > 1 are conventionally retained)
- **Rotation** (Varimax, Oblimin) a mathematical technique that makes the factor structure easier to interpret

**Example:** "EFA of the 24-item scale revealed four factors explaining 63% of total variance: Information Access, Search Strategy, Source Evaluation, and Ethical Use."

---

## Structural Equation Modeling (SEM)

**What it does:** Tests an entire theoretical model a network of relationships among multiple variables simultaneously. Combines factor analysis (measuring latent constructs) with path analysis (testing causal relationships among them).

**When to use it:** When you have a complex theoretical model with multiple mediators, moderators, or latent variables, and you want to test the entire model rather than one relationship at a time.

**Key concepts:**
- **Latent variables** constructs measured indirectly through multiple indicators (survey items)
- **Observed variables** the actual items or measurements
- **Path coefficients** the strength and direction of relationships between variables in the model
- **Model fit indices** statistics that tell you how well your theoretical model fits the data. Common ones: CFI (> .95 is good), RMSEA (< .06 is good), SRMR (< .08 is good)

```{warning}
SEM requires large samples (minimum 200, often 300+) and strong theoretical grounding. It's a powerful method but not appropriate for exploratory work or small samples.
```

---

## Multilevel Modeling (Hierarchical Linear Modeling / HLM)

**What it does:** Handles data with a nested structure individuals within groups, students within classrooms, library users within library systems. Standard regression assumes all observations are independent; multilevel modeling accounts for the fact that people in the same group are more similar to each other than to people in other groups.

**When to use it:** When your data has levels e.g., you surveyed librarians who are nested within library systems, or students who are nested within courses.

**Key concept:**
- **Intraclass Correlation Coefficient (ICC)** the proportion of total variance that exists *between* groups. If the ICC is near zero, there's no need for multilevel modeling. If it's substantial (> .05), ordinary regression may give you incorrect results.

---

## Analysis of Covariance (ANCOVA)

**What it does:** Compares groups on a DV while statistically controlling for one or more covariates. Essentially an ANOVA that adjusts for pre-existing differences between groups.

**When to use it:** When you want to compare groups but need to control for a confounding variable. For example, comparing two instructional methods while controlling for prior knowledge.

**Key concept:**
- **Adjusted means** the group means after the covariate has been statistically removed

---

## Nonparametric Tests: A Summary

When your data violate parametric assumptions (non-normal distributions, ordinal data, small samples), nonparametric tests are the alternative. They make fewer assumptions about the data but are generally less powerful (more likely to miss real effects).

| Parametric Test | Nonparametric Equivalent | Use When |
|----------------|-------------------------|----------|
| Independent t-test | **Mann-Whitney U** | 2 groups, ordinal or non-normal DV |
| Paired t-test | **Wilcoxon signed-rank** | Related groups, ordinal DV |
| One-way ANOVA | **Kruskal-Wallis H** | 3+ groups, ordinal or non-normal DV |
| Repeated measures ANOVA | **Friedman** | 3+ related measures, ordinal DV |
| Pearson correlation | **Spearman rₛ** | Ordinal data or non-linear relationships |

---

## Content Analysis Statistics

For researchers conducting quantitative content analysis (Krippendorff, 2018), several specific statistical measures are important:

**Krippendorff's alpha (α)**
: A reliability coefficient for content analysis that works with any number of coders, any number of categories, and any level of measurement. More robust than simpler alternatives like percent agreement or Cohen's kappa.

**Cohen's kappa (κ)**
: A measure of inter-rater agreement for two coders that corrects for chance agreement. Values above .80 are generally considered excellent; .60–.79 are acceptable.

**Scott's pi (π)**
: Similar to kappa but uses a different correction for chance. Less commonly used today.

---

## Network Analysis Statistics

For researchers studying social networks or information networks (Borgatti et al., 2018):

**Degree centrality** how many connections a node has

**Betweenness centrality** how often a node lies on the shortest path between other nodes (measures brokerage)

**Closeness centrality** how close a node is to all other nodes in the network

**Density** the proportion of possible connections that actually exist

**Clustering coefficient** the degree to which nodes tend to cluster together

---

## Where to Learn More

These methods are introduced briefly here as a reference. For deeper treatment, consult:

- **Field (2018)** *Discovering Statistics Using SPSS*: Comprehensive, accessible coverage of most methods listed above
- **Tabachnick & Fidell (2013)** *Using Multivariate Statistics*: The standard reference for regression, factor analysis, MANOVA, and other multivariate methods
- **Cohen (1992)** *A Power Primer*: Essential for understanding effect sizes and power analysis
- **Borgatti et al. (2018)** *Analyzing Social Networks*: For network-specific methods
- **Krippendorff (2018)** *Content Analysis*: For content analysis reliability and statistics
