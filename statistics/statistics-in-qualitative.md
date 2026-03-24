# Numbers in Qualitative Research

At first glance, "statistics" and "qualitative research" seem like they belong in different conversations. But qualitative researchers encounter quantitative concepts more often than they might expect. This chapter covers the specific places where numbers, measurement, and statistical thinking intersect with qualitative methodology.

---

## Inter-Rater Reliability in Qualitative Coding

When two or more researchers code the same data independently, you need a way to assess whether they agree. This is *inter-rater reliability* (or inter-coder agreement), and it involves quantitative measurement even in purely qualitative studies.

### Percent Agreement

The simplest measure: what percentage of coding decisions do the coders agree on?

**Example:** Two coders independently coded 50 text segments. They agreed on the code assignment for 42 of them. Percent agreement = 42/50 = 84%.

**Limitation:** Percent agreement doesn't account for the possibility that coders might agree *by chance*. If you have only two codes, coders would agree about 50% of the time even by guessing randomly.

### Cohen's Kappa (κ)

Corrects for chance agreement between two coders. This is the most commonly reported measure of inter-rater reliability in qualitative research.

| Kappa Value | Interpretation |
|-------------|---------------|
| < .20 | Poor agreement |
| .21 – .40 | Fair |
| .41 – .60 | Moderate |
| .61 – .80 | Substantial |
| .81 – 1.00 | Almost perfect |

### Krippendorff's Alpha

More flexible than kappa:  works with any number of coders (not just two), any number of categories, and any measurement level. Krippendorff (2018) recommends a minimum of α = .80, with α = .667 as the lowest acceptable value for tentative conclusions.

```{tip}
**What should you report in your methodology chapter?** If you use team coding, report your inter-rater reliability measure (kappa or Krippendorff's alpha), the number of coders, the percentage of data independently coded, and how disagreements were resolved. A common approach: independently code 20–25% of the data, calculate reliability, discuss and resolve disagreements, then code the remainder.
```

### The Debate About Reliability in Qualitative Research

Not all qualitative methodologists agree that inter-rater reliability is necessary or appropriate. Saldaña (2016) notes that some scholars question whether quantitative reliability measures are compatible with qualitative epistemology, since coding is inherently an interpretive act. These researchers prefer "dialogical intersubjectivity":  intensive group discussion and consensus:  over statistical coefficients.

Your committee's expectations will determine which approach you take. In either case, your methodology chapter should explain and justify your choice.

---

## Frequency Counts and Their Role

Counting how often a code appears across your data is a common:  and sometimes controversial:  practice in qualitative research.

### When Frequency Counts Help

- **Identifying dominant themes**: If a code appears in 18 of 20 interviews, that's analytically significant
- **Comparing across groups**: If a theme appears much more frequently in one subgroup, that pattern is worth exploring
- **Providing evidence for claims**: "Most participants described..." is strengthened by specifying "17 of 22 participants described..."
- **Content analysis**: In quantitative content analysis (Krippendorff, 2018), frequencies are a primary analytic tool

### When Frequency Counts Mislead

- **Frequency is not importance**: A theme mentioned once by one participant might be more analytically significant than a theme mentioned by everyone:  if it reveals something hidden or contradictory
- **Over-counting can flatten complexity**: Reducing rich qualitative data to frequency tables can strip away the context and nuance that make qualitative research valuable
- **Not all codes are equal**: A code that appears 30 times as brief mentions is different from a code that appears 5 times in deep, extended narratives

```{important}
Saldaña (2016) puts it directly: "Frequency of occurrence is not necessarily an indicator of significance." Use counts as *one* source of evidence, not the sole basis for your analysis. The strength of qualitative research lies in interpretation, not enumeration.
```

---

## Saturation: A Quasi-Statistical Concept

Theoretical saturation:  the point at which new data no longer generate new codes, categories, or themes:  is fundamentally a judgment call, but it has quantitative dimensions.

Guest, Bunce, and Johnson (2006) conducted one of the few empirical studies of saturation, finding that in their relatively homogeneous sample, 92% of codes were identified within the first 12 interviews. This is now widely cited as a benchmark, though the authors themselves caution against treating it as a universal rule.

### Reporting Saturation in Your Methodology Chapter

Rather than simply asserting "saturation was reached," consider providing evidence:

- Track new codes per interview and show the curve flattening
- Report the total number of codes at each stage of data collection
- Note when the last new code emerged relative to your final interview
- Acknowledge that saturation is a judgment, not a binary threshold

---

## Quantitizing: Transforming Qualitative Data into Numbers

In mixed methods research, "quantitizing" refers to converting qualitative data into numerical form for quantitative analysis (Saldaña, 2016). This can serve as a bridge between qualitative and quantitative strands.

### Common Approaches

**Magnitude coding**
: Assigning numerical values to qualitative ratings. For example, coding the intensity of a participant's expressed emotion on a 1–3 scale (mild, moderate, strong).

**Binary coding**
: Recording whether a theme is present (1) or absent (0) for each participant, creating a matrix that can be analyzed with chi-square or other statistical tests.

**Frequency matrices**
: Counting code frequencies by participant or by group, then comparing groups statistically.

### Paradigmatic Corroboration

Saldaña (2016) describes "paradigmatic corroboration":  when quantitative results from a dataset align with the qualitative coding of the same data, each validates the other. For example, if a t-test shows a significant difference between two groups' numeric ratings, and the qualitative codes for those groups also show distinct thematic patterns, the two forms of evidence corroborate each other.

---

## Descriptive Statistics That Qualitative Researchers Should Know

Even if you never run a statistical test, you'll encounter these concepts when reading quantitative research, participating in cross-method triad feedback, and communicating with committee members:

| Concept | Why It Matters for You |
|---------|----------------------|
| **Mean and standard deviation** | You'll see these in every quantitative study you read. Understanding what they communicate helps you critically evaluate findings. |
| **p-value** | Knowing what p < .05 means (and doesn't mean) is essential for reading research across traditions. See [Inferential Statistics](inferential-basics.md). |
| **Effect size** | Helps you evaluate whether a statistically significant finding is actually *meaningful*:  a skill useful in any tradition. |
| **Confidence interval** | Gives a range of plausible values rather than a single point estimate:  similar in spirit to qualitative researchers' comfort with multiple interpretations. |
| **Sample size and power** | Understanding why quantitative researchers need specific sample sizes helps you explain why qualitative research uses different:  and usually smaller:  samples. |
| **Correlation vs. causation** | A distinction that matters in both traditions. Qualitative researchers make causal claims through process tracing and thick description rather than through statistical control. |

---

## Using Statistics to Strengthen Qualitative Arguments

You don't need to *run* statistics to benefit from statistical thinking:

- **Be precise about quantities**: "Many participants" is weaker than "14 of 20 participants." Numbers add precision without sacrificing qualitative richness.
- **Contextualize your sample**: Provide demographic breakdowns (frequencies, percentages) so readers can assess transferability.
- **Acknowledge patterns quantitatively**: When you notice that a theme appears more in one subgroup, say so explicitly with counts.
- **Use visual displays**: Matrices and tables (Miles, Huberman, & Saldaña, 2014) bring systematic organization to qualitative data without reducing it to numbers.
- **Engage with quantitative literature**: Your literature review likely includes quantitative studies. Understanding their methods helps you synthesize across traditions.
