# Trees-analysis-identifies-patients-at-high-risk-for-kidney-function-decline

## Project Overview
This project focuses on identifying and analyzing influential predictors using advanced machine learning techniques, specifically random forest feature selection, logistic regression, and Classification and Regression Trees (CART).

## Methodology

### 1. Feature Selection: Random Forest
We employed random forest to perform initial feature selection and identify the most influential predictors in our dataset. Random forest offers several advantages:
- Handles non-linear relationships
- Provides feature importance rankings
- Reduces multicollinearity effects

#### Key Steps:
- Preprocessed and cleaned the dataset
- Applied random forest algorithm
- Ranked features based on their importance scores

### 2. Predictive Modeling

#### Logistic Regression
We used logistic regression to:
- Validate the selected features
- Estimate the probability of an outcome
- Quantify the impact of individual predictors

#### CART (Classification and Regression Tree)
CART was utilized to:
- Provide a tree-based interpretation of variable relationships
- Create a visual decision-making model
- Offer insights into non-linear interactions

## Project Workflow and RMarkdown Files

### 1. `1_preprocessing.rmd`
**Purpose**: Data Cleaning and Preparation
- Remove missing or inconsistent data
- Handle outliers
- Prepare dataset for further analysis
- Ensure data quality and reliability

### 2. `2_univariate_analysis.rmd`
**Purpose**: Initial Variable Exploration
- Conduct univariate analysis
- Perform logistic regression for continuous variables
- Run proportions test for binary indicators
- Provide initial insights into individual variable characteristics

### 3. `3_RF.rmd`
**Purpose**: Random Forest Feature Selection
- Fit random forest model
- Identify and rank top influential variables
- Determine feature importance
- Select most predictive features for further analysis

### 4. `4_DT.rmd`
**Purpose**: CART Decision Tree Analysis
- Develop Classification and Regression Tree model
- Visualize variable interactions
- Provide interpretable decision pathways
- Generate actionable insights for clinical researchers

### 5. `5_LR.rmd`
**Purpose**: Logistic Regression Modeling
- Conduct univariable logistic regression
- Perform multivariate logistic regression
- Quantify variable effects
- Assess statistical significance of predictors

## Recommended Workflow
1. Start with `1_preprocessing.rmd`
2. Run `2_univariate_analysis.rmd`
3. Execute `3_RF.rmd` for feature selection
4. Analyze results with `4_DT.rmd`
5. Validate findings using `5_LR.rmd`

## Result Interpretation

### Feature Importance
- **Random Forest Ranking**: Provides a quantitative measure of each variable's predictive power
- **Logistic Regression Coefficients**: Indicates the direction and magnitude of each predictor's effect
- **CART Tree Splits**: Reveals critical decision points and threshold values

### How to Read the Results
1. **Positive Coefficients**: Increase the likelihood of the target outcome
2. **Negative Coefficients**: Decrease the likelihood of the target outcome
3. **Feature Importance Scores**: Higher scores indicate more influential predictors

## Recommendations
- Carefully examine features with high importance scores
- Consider the context and domain knowledge when interpreting results
- Validate findings with domain experts

## Limitations
- Results are specific to the current dataset
- Potential for overfitting
- Requires periodic revalidation

## Dependencies
- R
- tidyverse
- caret
- randomForest
- rpart
- glmnet

## Dependencies
- R

## Contact
[Weihao Wang]
[weihao.wang@stonybrook.edu]
