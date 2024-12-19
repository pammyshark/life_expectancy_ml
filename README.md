# Life Expectancy Prediction Project

## Overview
This project analyzes and predicts life expectancy based on various health, social, and economic factors. The dataset used is sourced from the [WHO Life Expectancy Dataset](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who/data). The primary focus is on exploring the data, preprocessing it, engineering features, building regression models, and evaluating their performance.

---

## Project Components

### 1. Data Exploration and Understanding
- The dataset was loaded and its structure inspected to understand the data distribution and relationships among features.
- Independent (features) and dependent variables (target: `Life Expectancy`) were identified.
- Initial analysis included:
  - Examining the shape of the data
  - Checking for missing values
  - Inspecting data types of each column
  - Analyzing the distribution of the target variable with a histogram

---

### 2. Exploratory Data Analysis (EDA) and Data Preprocessing
- Missing values were handled as follows:
  - Numerical features were imputed with the mean.
  - Categorical features were imputed with the mode.
- Categorical variables were transformed into numerical representations through appropriate encoding technique (One-Hot Encoding).

---

### 3. Feature Engineering
- Several feature scaling techniques were applied (Standard Scaling, Min-Max Scaling, Robust Scaling), and the most suitable technique was finalized based on observations.
- A correlation matrix was calculated to identify the top 5 features most correlated with the target variable, which were documented for further analysis.

---

### 4. Model Building
- An initial train-test split of 60% training and 40% testing was used.
- Two regression models were built:
  - **Multiple Linear Regression**: This model utilized selected independent features to predict life expectancy. The best-fit line was plotted.
  - **Simple Linear Regression**: This model focused on the most important feature (from the correlation matrix) and its relationship with life expectancy. The best-fit line was also plotted.

---

### 5. Model Evaluation and Tuning
- The performance of both models was evaluated using the following metrics:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R-Squared (R²)
- The train-test split was modified to 80% training and 20% testing to observe performance improvements. Models were rebuilt and reevaluated.
- Cross-validation techniques were explored to further assess performance. The chosen method (Holdout, LOOCV, Stratified, or K-Fold) was applied, and its impact on model performance was documented with reasoning.

---

## How to Run the Project
1. Clone this repository.
2. Install the required Python packages (listed in `requirements.txt`).
3. Run the Jupyter Notebook or Python scripts to reproduce the analysis.

---

## Dataset Reference
- **Source**: [WHO Life Expectancy Dataset](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who/data)

---

## Acknowledgments
- Kaggle for providing the dataset.
- WHO for curating life expectancy statistics.

---

Contributions to improve this project are welcome!
