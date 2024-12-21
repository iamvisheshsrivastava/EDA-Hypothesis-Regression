# EDA-Hypothesis-Regression

Welcome to the **EDA-Hypothesis-Regression** repository! This repository encompasses a series of comprehensive statistical projects focusing on Exploratory Data Analysis (EDA), hypothesis testing, and regression analysis. Each project delves into real-world datasets, applying robust statistical methods to derive meaningful insights.

## Table of Contents

- [Projects Overview](#projects-overview)
  - [Project I: Descriptive Analysis of Demographic Data](#project-i-descriptive-analysis-of-demographic-data)
  - [Project II: Comparison of Multiple Distributions](#project-ii-comparison-of-multiple-distributions)
  - [Project III: Regression Analysis on Seoul Bike Sharing Data](#project-iii-regression-analysis-on-seoul-bike-sharing-data)
- [Tools and Technologies](#tools-and-technologies)
- [Data Sources](#data-sources)
- [Repository Structure](#repository-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Acknowledgments](#acknowledgments)
- [License](#license)
- [Contact](#contact)

---

## Projects Overview

This repository contains three major projects, each aimed at exploring different aspects of statistical analysis using R. Below is a detailed overview of each project.

### Project I: Descriptive Analysis of Demographic Data

**Objective:**  
Conduct a thorough descriptive analysis of demographic data with a focus on life expectancy and under-age-5 mortality rates across various countries.

**Dataset:**  
- **Source:** International Data Base (IDB) of the U.S. Census Bureau  
- **File:** `census2002_2022.csv`  
- **Description:**  
  Contains data on life expectancy at birth and under-age-5 mortality rates for 227 countries, spanning the years 2002 and 2022. The data is further stratified by sex and region.

**Tasks:**
1. **Frequency Distributions:**  
   Analyze the frequency distributions of life expectancy and mortality rates.
2. **Variability Comparison:**  
   Compare variability within subregions and between regions.
3. **Bivariate Correlations:**  
   Examine correlations between life expectancy and mortality rates.
4. **Temporal Analysis:**  
   Assess changes in life expectancy and mortality rates over the 20-year period (2002 vs. 2022).

**Methods Used:**
- Descriptive Statistics
- Variance Analysis
- Data Visualization (Box Plots, Histograms, Scatter Plots)

**Key Insights:**
- Trends in life expectancy improvements over two decades.
- Regional disparities in under-age-5 mortality rates.
- Correlations between life expectancy and mortality rates.

---

### Project II: Comparison of Multiple Distributions

**Objective:**  
Investigate the relationship between maternal smoking habits and newborn birth weights, assessing how different smoking categories influence birth weights.

**Dataset:**  
- **Source:** "Mothers and their Babies" data from Stat Labs  
- **File:** `MothersBabies.csv`  
- **Variables:**  
  - `wt`: Babies' birth weights (oz)  
  - `smoke`: Mothers' smoking history (categorical)

**Tasks:**
1. **Descriptive Analysis:**  
   Describe the distributions of birth weights (`wt`) and smoking categories (`smoke`).
2. **Hypothesis Testing:**  
   Test for significant differences in birth weights across different smoking categories using ANOVA and t-tests.
3. **Post-hoc Analysis:**  
   Conduct pairwise comparisons with Bonferroni and Tukey’s corrections to identify specific group differences.
4. **Method Comparison:**  
   Compare the results obtained from different correction methods against non-adjusted tests.

**Methods Used:**
- Hypothesis Testing (ANOVA, t-tests)
- Post-hoc Analysis (Bonferroni, Tukey’s HSD)
- Data Visualization (Box Plots, Confidence Intervals)

**Key Insights:**
- Impact of maternal smoking on newborn birth weights.
- Identification of specific smoking categories that significantly affect birth weights.
- Evaluation of statistical correction methods in multiple testing scenarios.

---

### Project III: Regression Analysis on Seoul Bike Sharing Data

**Objective:**  
Develop and evaluate regression models to predict bike-sharing demand in Seoul, leveraging various meteorological and temporal factors.

**Dataset:**  
- **Source:** Seoul Bike Sharing Demand Dataset  
- **File:** `Bikedata.csv`  
- **Variables:**  
  - **Dependent Variable:** `log.Rented.Bike.Count` (log-transformed)  
  - **Independent Variables:** Hour, Temperature, Humidity, Windspeed, Visibility, Solar Radiation, Rainfall, Snowfall, Seasons, Holiday

**Tasks:**
1. **Exploratory Data Analysis (EDA):**  
   Conduct EDA using scatter plots and correlation analysis to understand relationships between variables.
2. **Model Building:**  
   Develop a linear regression model to predict `log.Rented.Bike.Count`.
3. **Model Selection:**  
   Identify the best subset of predictors using criteria such as AIC, BIC, and Adjusted R².
4. **Model Evaluation:**  
   Assess the model's performance through residual analysis and multicollinearity diagnostics using Variance Inflation Factor (VIF).

**Methods Used:**
- Linear Regression
- Model Selection Techniques (AIC, BIC, Adjusted R²)
- Multicollinearity Diagnostics (VIF)
- Residual Analysis

**Key Insights:**
- Factors significantly influencing bike-sharing demand.
- Optimal model specifications for accurate predictions.
- Addressing multicollinearity to enhance model reliability.

---

## Tools and Technologies

- **Programming Language:** R  
- **Development Environment:** RStudio  
- **Key Libraries:**  
  - **Data Wrangling:** `dplyr`, `tidyr`  
  - **Visualization:** `ggplot2`, `gridExtra`, `corrplot`, `cowplot`, `ggpubr`  
  - **Statistical Analysis:** `car`, `MASS`, `lmtest`, `leaps`

## Data Sources

1. **International Data Base (IDB):**  
   Data on life expectancy and mortality rates.
   
2. **Mothers and Babies Dataset:**  
   Data on maternal smoking habits and newborn birth weights.
   
3. **Seoul Bike Sharing Demand Dataset:**  
   Data on bike-sharing usage and associated meteorological factors.

## Repository Structure

```
EDA-Hypothesis-Regression/
├── Project_I/
│   ├── ICS Project 1- Srivastava, Vishesh (230827).Rmd
│   ├── ICS Project 1- Srivastava, Vishesh (230828).pdf
│   ├── Vishesh_Srivastava_ICS_P2_Report.pdf
│   └── ...
├── Project_II/
│   ├── Vishesh_Srivastava_ICS_P2_code.Rmd
│   ├── Vishesh_Srivastava_ICS_P2_Report.pdf
│   └── ...
├── Project_III/
│   ├── Vishesh_Srivastava_ICS_P3_code.Rmd
│   ├── Vishesh_Srivastava_ICS_P3_Report.pdf
│   └── ...
├── census2002_2022.csv
├── MothersBabies.csv
├── Bikedata.csv
├── README.md
└── .gitattributes
```

- **Project_I, Project_II, Project_III:**  
  Each folder contains R Markdown files (`.Rmd`) and corresponding PDF reports detailing the analysis and findings.

- **Datasets:**  
  Raw datasets used in the projects.

- **.gitattributes:**  
  Git attribute settings for the repository.

## Installation

To get a local copy up and running, follow these simple steps:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/iamvisheshsrivastava/EDA-Hypothesis-Regression.git
   ```

2. **Navigate to the Project Directory:**

   ```bash
   cd EDA-Hypothesis-Regression
   ```

3. **Install Required R Packages:**

   Ensure you have R and RStudio installed. Open RStudio and install the necessary packages:

   ```R
   install.packages(c("dplyr", "tidyr", "ggplot2", "gridExtra", "corrplot", "cowplot", "ggpubr", "RColorBrewer", "car", "MASS", "lmtest", "leaps"))
   ```

## Usage

Each project is organized into its respective folder containing detailed code and reports. Follow the steps below to reproduce the analyses:

### Project I: Descriptive Analysis of Demographic Data

1. **Navigate to Project I Folder:**

   ```bash
   cd Project_I
   ```

2. **Open the R Markdown File:**

   Open `ICS Project 1- Srivastava, Vishesh (230827).Rmd` in RStudio.

3. **Run the Analysis:**

   Click on the "Knit" button in RStudio to generate the PDF report.

### Project II: Comparison of Multiple Distributions

1. **Navigate to Project II Folder:**

   ```bash
   cd Project_II
   ```

2. **Open the R Markdown File:**

   Open `Vishesh_Srivastava_ICS_P2_code.Rmd` in RStudio.

3. **Run the Analysis:**

   Click on the "Knit" button in RStudio to generate the PDF report.

### Project III: Regression Analysis on Seoul Bike Sharing Data

1. **Navigate to Project III Folder:**

   ```bash
   cd Project_III
   ```

2. **Open the R Markdown File:**

   Open `Vishesh_Srivastava_ICS_P3_code.Rmd` in RStudio.

3. **Run the Analysis:**

   Click on the "Knit" button in RStudio to generate the PDF report.

**Note:** Ensure that the datasets (`census2002_2022.csv`, `MothersBabies.csv`, `Bikedata.csv`) are placed in the root directory of the repository or update the file paths in the R Markdown files accordingly.

## Results

Each project generates detailed reports in PDF format, presenting the methodologies, analyses, results, and interpretations. Key visualizations include:

- **Box Plots and Histograms:**  
  For understanding distribution and variability in demographic data and birth weights.

- **Correlation Matrices and Scatter Plots:**  
  To identify relationships between variables in the bike-sharing dataset.

- **Regression Diagnostics:**  
  Including residual plots and VIF scores to validate regression models.

**Sample Visualization:**

![Sample Box Plot](images/sample_boxplot.png)

*(Ensure to include relevant images in an `images/` folder for visualization)*

## Acknowledgments

This work was completed as part of the coursework for the **Fakultät Statistik**, **TU Dortmund University** under the supervision of:

- **Prof. Dr. Katja Ickstadt**
- **M.Sc. Zeyu Ding**
- **M.Sc. Yassine Talleb**

I extend my gratitude for their invaluable guidance and support throughout these projects.

## License

Distributed under the [MIT License](LICENSE). See `LICENSE` for more information.

## Contact

- **Vishesh Srivastava**  
  [GitHub](https://github.com/iamvisheshsrivastava) | [Email](mailto:srivastava.vishesh9@gmail.com)

Feel free to reach out for any inquiries or collaborations!

---

© 2024 [GitHub](https://github.com/), Inc.

