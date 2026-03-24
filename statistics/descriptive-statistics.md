# Descriptive Statistics: Summarizing Your Data

Descriptive statistics do exactly what the name says — they *describe* your data. Before you run any inferential test, you need to understand what your data look like. Descriptive statistics are also what you report in your results section to give readers a picture of your sample and variables.

---

## Measures of Central Tendency

Central tendency answers the question: *What is the typical value?*

### Mean (Average)

The sum of all values divided by the number of values. The most common measure, but sensitive to extreme values (outliers).

**When to use:** Interval or ratio data that are approximately normally distributed.

**Example:** The mean number of database searches per session was 4.7 (*SD* = 2.3).

### Median

The middle value when all scores are arranged in order. Not affected by outliers.

**When to use:** Ordinal data, or interval/ratio data that are skewed.

**Example:** The median annual salary for respondents was $52,000 — more informative than the mean when a few very high salaries pull the average up.

### Mode

The most frequently occurring value. The only measure of central tendency appropriate for nominal data.

**When to use:** Nominal data, or to describe the most common category.

**Example:** The modal response for preferred search tool was "Google Scholar."

```{tip}
**Which one should you report?** For normally distributed interval/ratio data, report the mean. For skewed data, report the median (and mention the skew). For categorical data, report the mode or frequency counts. In your dissertation, you'll typically report the mean and standard deviation together: *M* = 3.82, *SD* = 0.91.
```

---

## Measures of Variability (Spread)

Central tendency alone is misleading without knowing how spread out the data are. Two datasets can have the same mean but look completely different.

### Range

The difference between the highest and lowest values. Simple but easily distorted by a single extreme value.

### Standard Deviation (SD)

The average distance of scores from the mean. This is the most commonly reported measure of spread. A small SD means scores cluster tightly around the mean; a large SD means they are widely dispersed.

**APA reporting format:** *M* = 3.82, *SD* = 0.91

### Variance

The standard deviation squared. Rarely reported directly, but it's the foundation of many statistical tests (ANOVA literally stands for "Analysis of Variance").

### Interquartile Range (IQR)

The range of the middle 50% of scores (the distance between the 25th and 75th percentiles). Useful for skewed data because it ignores the extremes.

---

## Frequency Distributions and Cross-Tabulations

For categorical variables, you describe data using counts and percentages rather than means:

**Frequency table example:**

| Library Type | Count | Percentage |
|-------------|-------|------------|
| Academic | 47 | 39.2% |
| Public | 42 | 35.0% |
| Special | 18 | 15.0% |
| School | 13 | 10.8% |
| **Total** | **120** | **100%** |

**Cross-tabulation** (contingency table) shows the relationship between two categorical variables — for example, library type by geographic region. Chi-square tests analyze these tables (see [Inferential Statistics](inferential-basics.md)).

---

## Visualizing Your Data

A well-chosen chart reveals patterns that numbers alone can miss. Different data types call for different visualizations:

| Data Type | Best Visualization | What It Shows |
|-----------|-------------------|---------------|
| One continuous variable | Histogram | Distribution shape, center, spread |
| One categorical variable | Bar chart | Frequency of categories |
| Two continuous variables | Scatterplot | Relationship between variables |
| Continuous by groups | Box plot | Center, spread, and outliers across groups |
| Change over time | Line graph | Trends and patterns |
| Parts of a whole | Stacked bar or pie chart | Proportions |

```{warning}
**Avoid pie charts for more than 4–5 categories** — they become unreadable. Use bar charts instead. Also, always start your y-axis at zero for bar charts to avoid visually exaggerating small differences.
```

---

## Describing Your Sample

The first table in most quantitative results sections is a **sample characteristics table** (sometimes called "Table 1"). It describes your participants on key demographic and background variables:

**Example format:**

| Characteristic | *n* | % |
|---------------|-----|---|
| **Gender** | | |
| Women | 87 | 72.5 |
| Men | 28 | 23.3 |
| Non-binary / not reported | 5 | 4.2 |
| **Highest Degree** | | |
| Bachelor's | 14 | 11.7 |
| Master's (MLIS or equivalent) | 89 | 74.2 |
| Doctorate | 17 | 14.2 |
| **Years of Experience** | | |
| *M* = 8.4, *SD* = 5.2, Range: 1–28 | | |

This table accomplishes two things: it helps readers assess whether your sample is relevant to their context (transferability), and it provides the data needed for others to compare their samples to yours.
