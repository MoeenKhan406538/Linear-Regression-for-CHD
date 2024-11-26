# Linear Regression on California Housing Data

This project demonstrates the implementation of a **Multiple Linear Regression** model to predict housing prices based on the features from the California housing dataset. The dataset includes various features such as median income, housing age, and proximity to the ocean, which influence housing prices.

## Project Overview

The goal of this project is to:
- Explore and preprocess the California housing dataset.
- Build a multiple linear regression model.
- Evaluate the model using metrics like **Mean Squared Error (MSE)** and **R-squared Error**.
- Perform residual analysis to validate model assumptions and improve its performance.

## Table of Contents
1. [Dataset](#dataset)
2. [Project Workflow](#project-workflow)
3. [Evaluation Metrics](#evaluation-metrics)
4. [Results](#results)
5. [Conclusions](#conclusions)

---

### Dataset

The dataset used in this project is the **California Housing dataset**, which is available via `scikit-learn`. It includes the following features:
- Median income
- House age
- Average rooms
- Average bedrooms
- Population
- Latitude and Longitude

The target variable is the **median house value**.

---

### Project Workflow

1. **Data Preprocessing:**
   - Handling missing values.
   - Splitting the dataset into training and testing sets.
   - Feature scaling using **Min-Max Scaling** to normalize data for better performance.

2. **Model Training:**
   - Training a **Multiple Linear Regression** model using the `LinearRegression` class from `scikit-learn`.

3. **Model Evaluation:**
   - Calculating performance metrics: **Mean Squared Error** and **R-squared Error**.
   - Analyzing residual plots to validate assumptions like homoscedasticity and normality of residuals.

4. **Optimization:**
   - Exploring scaling techniques to optimize performance.
   - Attempted improvements based on residual analysis.

---

### Evaluation Metrics

- **Mean Squared Error (MSE):** Measures the average squared difference between actual and predicted values.  
  MSE for this model: **4,852,059,947.13**

- **R-squared Error:** Represents the proportion of variance explained by the model.  
  R-squared for this model: **0.630**

---

### Results

- The model achieved reasonable performance given the complexity of the dataset and the nature of the task.
- Residual analysis showed a nearly random pattern, suggesting that the model assumptions hold relatively well.

---

### Conclusions

- **Strengths:**  
  The model captures a significant amount of variance in the target variable and demonstrates the predictive power of features like median income and location.

- **Limitations:**  
  - The R-squared score indicates room for improvement, likely due to non-linear relationships or omitted variables.  
  - High MSE suggests potential outliers or extreme values influencing the predictions.
