# EDA, Hypothesis Testing, and Regression Projects

This repository collects three R-based statistics projects covering exploratory data analysis, hypothesis testing, and regression modeling. Each project folder contains the report source and supporting outputs.

## Projects

### Project I: Demographic data analysis

- descriptive analysis of life expectancy and under-age-5 mortality
- comparisons across regions and over time

### Project II: Smoking and birth weight

- hypothesis testing across maternal smoking categories
- ANOVA, pairwise tests, and multiple-comparison corrections

### Project III: Seoul bike sharing regression

- linear regression for bike-demand modeling
- model selection, diagnostics, and multicollinearity checks

## Repository layout

```text
EDA-Hypothesis-Regression/
|-- Project_I/
|-- Project_II/
|-- Project_III/
`-- README.md
```

## Tools

- R
- RStudio
- dplyr
- tidyr
- ggplot2
- car
- MASS
- lmtest
- leaps

## Getting started

1. Clone the repository.
2. Open the relevant `.Rmd` file in RStudio.
3. Install the required packages.
4. Knit the report or run the notebook cells interactively.

## Example package install

```r
install.packages(c(
  "dplyr",
  "tidyr",
  "ggplot2",
  "gridExtra",
  "corrplot",
  "cowplot",
  "ggpubr",
  "RColorBrewer",
  "car",
  "MASS",
  "lmtest",
  "leaps"
))
```

## Notes

- The projects were completed as part of coursework at TU Dortmund University.
- File and report names are preserved from the original submissions.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
