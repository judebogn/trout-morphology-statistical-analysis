# Trout Morphology: Exploratory and Inferential Analysis

A reproducible R Markdown project studying morphological measurements from two trout species sampled across three lakes. The project demonstrates data preparation, exploratory analysis, visualization, statistical testing, and interpretation.

## View the analysis

- **`analysis.Rmd`** is the source document containing the R code, tables, plots, and explanations.
- Knit `analysis.Rmd` to **GitHub Markdown** to create `analysis.md`. GitHub can display the generated Markdown, including embedded plots, directly in the repository.

To render the report in RStudio, open `analysis.Rmd` and click **Knit**, or run:

```r
rmarkdown::render("analysis.Rmd")
```

The document is configured to generate GitHub-flavoured Markdown. After knitting, commit both `analysis.Rmd` and the generated `analysis.md` (as well as the generated figure folder) so visitors can read the results without running R themselves.

## Research questions

- How are body length, jaw length, and number of spots distributed?
- Do body and jaw lengths differ between the two species?
- Does the number of spots differ between species?
- Is species associated with lake of origin?
- How strongly are body length and jaw length related?

## Dataset

The dataset contains 306 observations and six variables: individual ID, species, lake, number of spots, body length (mm), and jaw length (mm).

The number of spots is treated as a variable supplied in the academic assignment; any interpretation of it as a stress indicator would require independent biological validation.

## Methods

- Data import and quality checks
- Descriptive statistics and group summaries
- Histograms, boxplots, and scatterplots
- Welch two-sample t-tests for body and jaw lengths
- Wilcoxon rank-sum test for number of spots
- Fisher's exact test for species-by-lake association
- Pearson correlation for body and jaw lengths, including species-specific correlations

## Requirements

R (4.2 or later recommended) and the packages `rmarkdown`, `knitr`, `readr`, `dplyr`, and `ggplot2`. Install them with:

```r
install.packages(c("rmarkdown", "knitr", "readr", "dplyr", "ggplot2"))
```

## Limitations

This is an exploratory academic analysis of one supplied dataset, not a causal study. Species and lake may be associated, multiple tests are conducted, and the pooled correlation may partly reflect differences between species. Results should therefore be interpreted with the sampling design, effect sizes, and uncertainty in mind.

## Authors

- Mahoulé Jude Bogninou
- Laetitia Yangouen Nankam (co-author of the original academic project)

Before publishing publicly, confirm that both authors agree and that the course rules allow redistribution of the data. No license is included until redistribution rights are confirmed.
