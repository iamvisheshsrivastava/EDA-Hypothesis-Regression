## Projects Overview

### **Project I: Descriptive Analysis of Demographic Data**
- **Objective**: Analyze demographic data focusing on life expectancy and mortality rates.
- **Dataset**: Extracted from the [International Data Base (IDB)](https://www.census.gov/programs-surveys/international-programs/about/idb.html) of the U.S. Census Bureau.
  - File: `census2002_2022.csv`
  - Contains life expectancy at birth and under-age-5 mortality rates for 227 countries (2002 and 2022), stratified by sex and region.
- **Tasks**:
  1. Describe frequency distributions of variables (life expectancy and mortality rates).
  2. Compare variability within subregions and between regions.
  3. Analyze bivariate correlations between variables.
  4. Examine changes over 20 years (2002 vs. 2022).
- **Methods Used**: Descriptive statistics, variance analysis, and visualization (bar plots, box plots, scatter plots).

---

### **Project II: Comparison of Multiple Distributions**
- **Objective**: Investigate the relationship between maternal smoking habits and newborn weights.
- **Dataset**: "Mothers and their Babies" data sourced from [Stat Labs](https://www.stat.berkeley.edu/users/statlabs/labs.html).
  - Cleaned version available as `MothersBabies.csv`.
  - Variables:
    - `wt`: Babies' birth weights (oz).
    - `smoke`: Mothers' smoking history (categorical).
- **Tasks**:
  1. Describe distributions of `wt` and `smoke`.
  2. Test for global differences in babies' weights across smoking categories.
  3. Conduct pairwise comparisons (two-sample tests) with Bonferroni and Tukey’s corrections.
  4. Compare results of correction methods with non-adjusted tests.
- **Methods Used**: Hypothesis testing (ANOVA, t-tests), post-hoc analysis, visualization (box plots, confidence intervals).

---

### **Project III: Regression Analysis on Seoul Bike Sharing Data**
- **Objective**: Build and evaluate regression models to predict bike-sharing demand.
- **Dataset**: [Seoul Bike Sharing Demand Dataset](https://archive.ics.uci.edu/ml/datasets/Seoul+Bike+Sharing+Demand).
  - Modified version: `Bikedata.csv`
  - Dependent Variable: `log.Rented.Bike.Count` (log-transformed).
  - Independent Variables: Hour, Temperature, Humidity, Windspeed, Visibility, Solar Radiation, Rainfall, Snowfall, Seasons, Holiday.
- **Tasks**:
  1. Perform EDA (scatter plots, correlation analysis).
  2. Build a linear regression model for `log.Rented.Bike.Count`.
  3. Select the best subset of predictors (AIC, BIC, Adjusted R²).
  4. Evaluate the model using residual plots and variance inflation factor (VIF).
- **Methods Used**: Linear regression, model selection, multicollinearity diagnostics, residual analysis.

---

## Tools and Programming
- **Language**: R (RStudio)
- **Libraries**:
  - Data Wrangling: `dplyr`, `tidyr`
  - Visualization: `ggplot2`, `gridExtra`
  - Statistical Analysis: `car`, `MASS`, `lmtest`

---

## Data Sources
- [International Data Base (IDB)](https://www.census.gov/programs-surveys/international-programs/about/idb.html)
- [Mothers and Babies Dataset](https://www.stat.berkeley.edu/users/statlabs/labs.html)
- [Seoul Bike Sharing Demand Dataset](https://archive.ics.uci.edu/ml/datasets/Seoul+Bike+Sharing+Demand)

---

## How to Use This Repository
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/your_username/Statistical-Projects-TU-Dortmund.git
   ```
2. Navigate to the respective project folders for detailed code and analysis:
   - **Project_I**: Descriptive Analysis
   - **Project_II**: Comparison of Distributions
   - **Project_III**: Regression Analysis
3. Open and run `.R` files in RStudio for reproducibility.

---

## Acknowledgments
This work was completed as part of the coursework for **Fakultät Statistik, TU Dortmund University** under the supervision of:
- **Prof. Dr. Katja Ickstadt**
- **M.Sc. Zeyu Ding**
- **M.Sc. Yassine Talleb**

I am grateful for their guidance and support throughout these projects.

