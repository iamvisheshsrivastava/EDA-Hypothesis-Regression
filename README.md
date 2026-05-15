# EDA, Hypothesis Testing & Regression

**[View the project showcase →](https://iamvisheshsrivastava.github.io/EDA-Hypothesis-Regression)**

Three end-to-end statistical analysis projects built in R as part of coursework at TU Dortmund University. Each project covers a different pillar of applied statistics — from exploratory analysis and hypothesis testing to regression modeling and diagnostics.

---

## Projects

### Project I — Demographic Data Analysis
Descriptive and visual analysis of global life expectancy and under-age-5 mortality. Explores patterns across world regions and tracks trends over time.

| File | Description |
|------|-------------|
| [`Project_I/Vishesh_Srivastava_ICS_P1_code.Rmd`](Project_I/Vishesh_Srivastava_ICS_P1_code.Rmd) | R Markdown source |
| [`Project_I/Vishesh_Srivastava_ICS_P1_Report.pdf`](Project_I/Vishesh_Srivastava_ICS_P1_Report.pdf) | Final report (PDF) |

### Project II — Smoking & Birth Weight
Investigates the effect of maternal smoking on infant birth weight using one-way ANOVA, Kruskal-Wallis tests, and pairwise comparisons with Bonferroni and Tukey corrections.

| File | Description |
|------|-------------|
| [`Project_II/Vishesh_Srivastava_ICS_P2_code.Rmd`](Project_II/Vishesh_Srivastava_ICS_P2_code.Rmd) | R Markdown source |
| [`Project_II/Vishesh_Srivastava_ICS_P2_Report.pdf`](Project_II/Vishesh_Srivastava_ICS_P2_Report.pdf) | Final report (PDF) |

### Project III — Seoul Bike Sharing Demand
Builds and evaluates a linear regression model to predict hourly bike rentals. Covers variable selection, multicollinearity (VIF), residual diagnostics, Box-Cox transformation, and influential point analysis.

| File | Description |
|------|-------------|
| [`Project_III/Vishesh_Srivastava_ICS_P3_code.Rmd`](Project_III/Vishesh_Srivastava_ICS_P3_code.Rmd) | R Markdown source |
| [`Project_III/Vishesh_Srivastava_ICS_P3_Report.pdf`](Project_III/Vishesh_Srivastava_ICS_P3_Report.pdf) | Final report (PDF) |

---

## Stack

`R` · `RStudio` · `ggplot2` · `dplyr` · `tidyr` · `car` · `MASS` · `lmtest` · `leaps`

---

## Getting Started

```r
# Install all required packages
install.packages(c(
  "dplyr", "tidyr", "ggplot2", "gridExtra",
  "corrplot", "cowplot", "ggpubr", "RColorBrewer",
  "car", "MASS", "lmtest", "leaps"
))
```

1. Clone the repo
2. Open the relevant `.Rmd` file in RStudio
3. Knit the report or run cells interactively

---

## License

[MIT](LICENSE)
