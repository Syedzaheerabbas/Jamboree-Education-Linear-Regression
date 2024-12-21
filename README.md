# Jamboree-Education-Linear-Regression
![image](https://github.com/user-attachments/assets/6f4ad165-4523-4246-b84e-6b5be9509b7b)


This project analyzes factors influencing graduate admissions to Ivy League colleges from an Indian perspective, using data provided by Jamboree, an overseas education consultancy. The goal is to understand the relationships between various applicant attributes and their chances of admission, and to build a predictive model.

## Project Overview

Jamboree aims to help students gain admission to top universities abroad. They recently launched a feature on their website to estimate the probability of Indian students getting into Ivy League graduate programs. This project supports that initiative by:

1.   **Data Loading and Preprocessing:** Importing the dataset and handling any missing values or irrelevant columns (like the serial number).
2.  **Exploratory Data Analysis (EDA):**
    *   Descriptive statistics (mean, median, standard deviation, etc.).
    *   Data visualizations (histograms, scatter plots, correlation matrices).
    *   Analysis of variable distributions and relationships.
3.  **Linear Regression Modeling :**
    *   Building a linear regression model using `statsmodels.api.OLS`.
    *   Interpreting the model summary, including coefficients, p-values, R-squared, and other statistics.
4.  **Regularized Regression (Scikit-learn):**
    *   Implementing Ridge and Lasso regression using `sklearn.linear_model.Ridge` and `sklearn.linear_model.Lasso`.
    *   Comparing the performance of regularized models with the basic linear regression model.
    *   (Optional) Tuning hyperparameters (alpha) for Ridge and Lasso using cross-validation (`sklearn.model_selection.GridSearchCV` or `RandomizedSearchCV`).
5.  **Model Diagnostics (Statsmodels):**
    *   Checking for multicollinearity using Variance Inflation Factor (VIF) (can be calculated using `statsmodels` or `statsmodels.stats.outliers_influence.variance_inflation_factor` or a custom function).
    *   Analyzing residuals for linearity, homoscedasticity, and normality using diagnostic plots and tests provided by `statsmodels`.
6.  **Model Evaluation:**
    *   Calculating metrics like Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), R-squared (R²), and Adjusted R² for all models (Linear, Ridge, Lasso) using `sklearn.metrics` or manual calculations.
7.  **Insights and Recommendations:** Drawing conclusions based on the analysis and providing actionable recommendations to Jamboree.


## Dataset

The dataset used in this project is `jamboree_admission.csv`, which contains the following features:

*   **GRE Scores:** Graduate Record Examinations score (out of 340).
*   **TOEFL Scores:** Test of English as a Foreign Language score (out of 120).
*   **University Rating:** University rating (out of 5).
*   **Statement of Purpose and Letter of Recommendation Strength:** Rating of the statement of purpose and letters of recommendation (out of 5).
*   **Undergraduate GPA:** Undergraduate Grade Point Average (out of 10).
*   **Research Experience:** Binary variable indicating research experience (0 or 1).
*   **Chance of Admit:** The target variable, representing the probability of admission (ranging from 0 to 1).

The dataset was provided by Jamboree.

## Methodology

The project follows these steps:

1.  **Data Loading and Preprocessing:** Importing the dataset and handling any missing values or irrelevant columns (like the serial number).
2.  **Exploratory Data Analysis (EDA):**
    *   Descriptive statistics (mean, median, standard deviation, etc.).
    *   Data visualizations (histograms, scatter plots, correlation matrices).
    *   Analysis of variable distributions and relationships.
3.  **Linear Regression Modeling:**
    *   Building a linear regression model using the `statsmodels` library.
    *   Interpreting the model coefficients and statistical significance.
4.  **Model Diagnostics:**
    *   Checking for multicollinearity using Variance Inflation Factor (VIF).
    *   Analyzing residuals for linearity, homoscedasticity, and normality.
5.  **Model Evaluation:**
    *   Calculating metrics like Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), R-squared (R²), and Adjusted R².
6.  **Insights and Recommendations:** Drawing conclusions based on the analysis and providing actionable recommendations to Jamboree.

## Libraries Used

*   pandas
*   numpy
*   matplotlib
*   seaborn
*   statsmodels
*   scikit-learn (potentially for VIF calculation and Model Building)

## Results and Insights 

*   **Strong Predictors:** CGPA (Undergraduate GPA), GRE scores, and TOEFL scores are significant predictors of admission chances. Higher scores in these areas are strongly correlated with a higher probability of admission.
*   **Positive Impact of Research:** Research experience has a positive impact on admission chances. Applicants with research experience tend to have a higher likelihood of being admitted.
*   **Model Performance:** The linear regression model achieved a good performance with an R-squared (R²) score of approximately 0.80. This indicates that the model explains a substantial portion (80%) of the variance in admission chances based on the included predictor variables.

## Recommendations for Jamboree

*   **Emphasize Key Metrics:** In their counseling sessions, Jamboree can emphasize the importance of achieving high scores in CGPA, GRE, and TOEFL. These are clearly crucial factors for admission.
*   **Support Statement of Purpose and Recommendations:** Jamboree can provide resources to help students improve their statement of purpose and letters of recommendation. This could include workshops, writing guides, or feedback sessions.
*   **Invest in Key Support Areas:** Jamboree should allocate additional resources to support critical areas such as GRE/TOEFL preparation and research opportunities. This could involve offering specialized test preparation courses, connecting students with research mentors or institutions, or providing funding for research projects. This investment will directly help students excel and improve their admission prospects.
*   **Targeted Counseling:** Jamboree could use the model to provide more personalized advice to students. By inputting a student's profile (CGPA, GRE, TOEFL, etc.), they could get an estimated probability of admission and tailor their recommendations accordingly.
*   **Further Investigation:** While the model performs well, further investigation could explore other potential factors that influence admissions (e.g., quality of the statement of purpose, specific university requirements).


## Further Improvements 

*   Collect more data to improve the model's accuracy and generalizability.
*   Deploy the model as a web application for Jamboree's website.

## Colab Notebook
- You can access the full Python analysis on Google Colab using the following link: [View the notebook](https://colab.research.google.com/drive/1K87JOiTTbnVGQcna-IO3bSItAgQj1jn1#scrollTo=BNbt-qGtjvxh)

## PDF Report

A detailed analysis report is available in the following PDF file: [View Report](Risk_anlytics.pdf).

## Contact

[SYED ZAHEER ABBAS] - [SYEDZAHEER.C@GMAIL.COM]
