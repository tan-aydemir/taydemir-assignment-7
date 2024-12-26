# Hypothesis Testing and Confidence Intervals in Linear Regression

## Project Overview

In this project, I extended my prior work on linear regression by incorporating hypothesis testing and confidence intervals through simulations. The objective was to develop an interactive web application that enables users to test the statistical significance of regression parameters—namely the slope and intercept—and generate confidence intervals based on simulated data. This project offered valuable hands-on experience in statistical analysis and reinforced my understanding of the impact of randomness on regression estimates.

## Key Features

### 1. **Interactive Web Application**
The web application provides an intuitive interface that allows users to interact with and explore the statistical properties of linear regression. The application includes several components:

#### **Data Generation Inputs:**
- **Intercept (β₀):** The true intercept of the regression line.
- **Slope (β₁):** The true slope of the regression line.
- **Mean (μ):** The mean of the normal error term added to the dependent variable (Y).
- **Variance (σ²):** The variance of the error term in the regression model.
- **Sample Size (N):** The number of data points to generate in the dataset.
- **Number of Simulations (S):** The number of datasets to simulate.

After users input the necessary parameters, the application generates:
- A **scatter plot** displaying the generated data points with random noise.
- **Histograms** showing the distribution of simulated slopes and intercepts from multiple datasets.

#### **Hypothesis Testing:**
Building on the data generation feature, users can test the statistical significance of the regression parameters. The application allows users to:
- **Select the parameter to test:** Either the slope or intercept.
- **Choose the type of test:** 
  - Greater than ( > )
  - Less than ( < )
  - Not equal to ( ≠ )
- After specifying these parameters, users can run the hypothesis test and obtain:
  - The **p-value** corresponding to the test.
  - A **histogram** of simulated statistics with the observed statistic and the hypothesized value visibly marked.

The p-value is calculated by comparing the observed statistic to the distribution of simulated statistics under the null hypothesis.

#### **Confidence Intervals:**
Users can also generate **confidence intervals** for the regression parameters:
- **Select the parameter** for which the confidence interval should be calculated (either slope or intercept).
- **Choose a confidence level** (e.g., 90%, 95%, or 99%).
- Upon clicking the "Calculate Confidence Interval" button, the application:
  - Computes the confidence interval for the selected parameter using the simulations.
  - Plots individual simulated estimates as gray points, with the **mean estimate** highlighted in color, and the **confidence interval** shown as a horizontal line.
  - Marks the true parameter value on the plot and colors the confidence interval based on whether it contains the true value.

### 2. **Additional Features**
- **Small p-values Handling:** The application includes a feature that displays a fun, informative message when a p-value is extremely small (≤ 0.0001), indicating a rare event in statistical terms.
- **Visualization and Analysis:** The app provides clear visualizations of how changes in parameters affect the distribution of simulated slopes and intercepts, as well as the resulting p-values and confidence intervals.

## Project Highlights

- **Hands-on Statistical Analysis:** The project allowed me to apply my understanding of hypothesis testing and confidence intervals within the context of linear regression, while reinforcing key concepts such as p-values and the interpretation of confidence intervals.
- **Web Application Development:** By developing this interactive web application, I gained practical experience in full-stack development using **Flask** and **JavaScript**, as well as data visualization using **Matplotlib** and **Plotly**.
- **Exploring Statistical Variability:** I observed firsthand how random noise can influence regression estimates, even when no true relationship exists between the variables, and how different sample sizes and noise levels affect the precision of the estimates.

## Conclusion

This project provided a chance to deepen my understanding of statistical analysis, particularly in the context of linear regression. By simulating different datasets and performing hypothesis testing and confidence interval estimation, I gained valuable insights into the effects of randomness and sample variability. The project also allowed me to strengthen my web development skills, especially in building interactive tools for data analysis.
