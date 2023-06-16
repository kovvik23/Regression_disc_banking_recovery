# Regression Discontinuity: Banking Recovery

This repository contains a Jupyter Notebook project that explores the concept of regression discontinuity in the context of banking recovery. The project is an extension of a [DataCamp project](https://www.datacamp.com/projects/504), focusing on determining whether the incremental amount the bank earns from assigning delinquent customers to a higher recovery strategy exceeds the additional cost.

## Dataset
The project uses a dataset called `bank_data.csv`, which contains information about the expected and actual recovery amounts for bank accounts. The dataset also includes variables such as customer age, sex, and recovery strategy level. This dataset is provided as part of the DataCamp project and serves as the foundation for the analysis. You can find the `bank_data.csv` file in the "dataset" folder within this repository.

## Project Overview
The project is divided into several sections, following the structure of the original DataCamp project with some extensions:

1. **Regression Discontinuity**: This section provides an introduction to the project and the concept of regression discontinuity. It explains the recovery strategies implemented by the bank at different thresholds and poses the main question of whether there is a jump in the recovery amount at the higher strategy level.

2. **Graphical Exploratory Data Analysis**: In this section, scatter plots are used to visually examine the relationship between the expected recovery amount and the actual recovery amount, as well as the customer age. The focus is on the range just below and above the threshold to identify any discontinuity.

3. **Statistical Test: Age vs. Expected Recovery Amount**: This section performs a statistical test using the Kruskal-Wallis One-Way ANOVA test to determine if there is a difference in customer age just above and below the threshold. The results help assess whether age varies smoothly or shows a discontinuity.

4. **Statistical Test: Sex vs. Expected Recovery Amount**: A chi-square test is conducted to examine the difference in the number of male and female customers above and below the threshold. The analysis determines if there is a statistically significant difference in the sex of the population.

5. **Graphical Exploratory Data Analysis of Actual vs. Expected Recovery Amount**: This section focuses on the selected range around the threshold to observe any potential discontinuity in the relationship between the actual and expected recovery amounts.

6. **Statistical Analysis: Recovery Amount**: Statistical tests, including the Kruskal-Wallis test, are performed to assess if there is a significant difference in the median actual recovery amounts above and below the threshold. The analysis is conducted for two different ranges of expected recovery amounts.

7. **Regression Modeling: No Threshold**: Two regression models are built to estimate the program impact at the $1000 threshold. The first model predicts the actual recovery amount solely based on the expected recovery amount. The adjusted R-squared value is used to evaluate the model's performance.

The project builds upon the foundation of the DataCamp project and extends the analysis in the statistical analysis section to provide additional insights.

## Usage
To run the project, you need to have Jupyter Notebook installed. You can then open the Jupyter Notebook file `regression_discontinuity_banking_recovery.ipynb` and execute the code cells sequentially.

Make sure to place the `bank_data.csv` file in the same directory as the Jupyter Notebook file (in the "dataset" folder within the repository) for the data to be loaded correctly.

## Dependencies
The following Python libraries are used in this project:
- pandas
- numpy
- matplotlib
- scipy
- statsmodels

You can install these dependencies using `pip` or any other package manager of your choice.

Please note that since the dataset used in this project is sourced from Datacamp and is not described in detail, the validity of the conclusions drawn from the analysis cannot be confirmed. Additionally, it's important to consider that the code and results may not reflect the most current information or trends in the field.
