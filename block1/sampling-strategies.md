# Sampling Strategies Across Traditions

## Sampling as a Design Decision

Sampling is not merely a procedural step-it is a *design decision* that shapes the scope, credibility, and transferability of your findings. The logic of sampling differs fundamentally across research traditions, and your methodology chapter must explain not only *who* you will study but *why* and *how* you selected them.

---

## Probability Sampling (Quantitative Tradition)

Probability sampling aims for *representativeness*-the ability to generalize findings from a sample to a larger population. Each member of the population has a known, non-zero probability of selection.

### Common Probability Sampling Techniques

**Simple random sampling**
: Every member has an equal chance of selection. Gold standard but often impractical for large or dispersed populations.

**Stratified random sampling**
: Population divided into homogeneous subgroups (strata), then random sampling within each. Ensures representation of key subgroups. Krippendorff (2018) notes this is particularly useful when distinct subpopulations need proportional representation.

**Cluster sampling**
: Naturally occurring groups (schools, districts, libraries) are randomly selected, then members within clusters are studied. Cost-effective for geographically dispersed populations.

**Systematic sampling**
: Every *k*th unit from a list after a random start. Efficient but can introduce bias if the list has a periodic pattern.

```{warning}
Krippendorff (2018) demonstrates how systematic sampling can create hidden bias. Selecting every 7th issue of a daily newspaper, for example, would always sample the same day of the week, potentially missing content that appears on other days.
```

---

## Purposive Sampling (Qualitative Tradition)

In qualitative research, the goal is not representativeness but *information richness* (Patton, 2014). Participants are selected deliberately because they can illuminate the phenomenon under study.

### Patton's (2014) Purposive Sampling Strategies

**Maximum variation**
: Deliberately selecting cases that span the range of variation on dimensions of interest. Identifies common patterns that cut across diversity.

**Homogeneous**
: Selecting participants who share key characteristics. Useful for focused inquiry into a specific subgroup's experience.

**Criterion**
: All cases that meet a predetermined criterion of importance. Ensures quality assurance.

**Snowball / Chain**
: Initial participants refer the researcher to others. Useful for hidden or hard-to-reach populations.

**Theory-based / Theoretical sampling**
: Selection driven by emerging theoretical constructs (Charmaz, 2006). Sampling continues until *theoretical saturation*-new data no longer generate new conceptual insights.

**Critical case**
: Selecting cases that are particularly important or revealing-if it holds here, it likely holds elsewhere.

**Intensity**
: Information-rich cases that manifest the phenomenon intensely but not extremely.

```{admonition} Key Reading
:class: seealso
Robinson (2013) provides an excellent practical framework for sampling in interview-based qualitative research, including a four-point approach to defining the sample universe, selecting a sampling strategy, determining sample size, and sourcing participants.
```

---

## Sample Size Considerations

Sample size logic differs dramatically between traditions.

### Quantitative: Power Analysis

Sample size is determined *a priori* through **power analysis**-calculating the number of participants needed to detect an effect of a given size with specified statistical power and significance level (Cohen, 1992).

Four parameters are interdependent:
1. **Effect size** (*d*, *r*, *f*): How large is the effect you expect to find?
2. **Alpha** (α): Your significance threshold (conventionally .05)
3. **Power** (1 - β): The probability of detecting a real effect (conventionally .80)
4. **Sample size** (*N*): Calculated from the other three

```{admonition} Cohen's (1992) Conventional Effect Sizes
:class: note

| Test | Small | Medium | Large |
|------|-------|--------|-------|
| t-test (*d*) | 0.20 | 0.50 | 0.80 |
| Correlation (*r*) | 0.10 | 0.30 | 0.50 |
| ANOVA (*f*) | 0.10 | 0.25 | 0.40 |
| Chi-square (*w*) | 0.10 | 0.30 | 0.50 |
```

Bartlett, Kotrlik, and Higgins (2001) provide practical tables and formulas for determining sample size in organizational research, complementing Cohen's statistical approach.

See the {doc}`notebook-power-analysis` for an interactive power analysis calculator.

### Qualitative: Saturation

Sample size is determined by **saturation**-the point at which additional data collection yields diminishing new insights. Guest, Bunce, and Johnson (2006) found that saturation often occurs within 12 interviews for relatively homogeneous populations, though this varies widely depending on the complexity of the phenomenon and the heterogeneity of participants.

```{tip}
In your methodology chapter, don't just state a sample size number-*justify* it. For quantitative work, report your power analysis parameters. For qualitative work, explain your saturation logic and cite methodological literature supporting your estimate.
```

### Mixed Methods: Dual Justification

Mixed methods research requires separate sampling justifications for each strand. Teddlie and Yu (2007) provide a comprehensive typology:

1. **Basic MM sampling**: Combining probability and purposive techniques
2. **Sequential MM sampling**: Information from the first strand informs sampling in the second
3. **Concurrent MM sampling**: Probability and purposive samples drawn simultaneously
4. **Multilevel MM sampling**: Different techniques applied at different levels of analysis

---

## ✏️ Exercise: Define Your Sampling Strategy

For your Block 1 deliverable, draft a sampling section (1–2 pages) that addresses:

1. **Population description**: Who is your target population? How do you define its boundaries?
2. **Sampling technique**: Which strategy will you use and why? (Cite methodological sources)
3. **Sample size justification**:
   - *Quantitative*: Report your power analysis (test, effect size, alpha, power, required N)
   - *Qualitative*: Discuss saturation; estimate initial sample size with rationale
   - *Mixed methods*: Provide separate justifications for each strand
4. **Recruitment procedures**: How will you identify and recruit participants?
5. **Inclusion/exclusion criteria**: Who is eligible? Who is not? Why?
6. **Anticipated challenges**: Access barriers, anticipated response rates, attrition
