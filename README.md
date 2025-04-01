# Diabetes Data Analysis and Prediction

This project performs exploratory data analysis (EDA) and builds a classification model on the Pima Indians diabetes dataset. It aims to uncover diabetes patterns and predict diabetes outcomes, focusing on a community known to have a predisposition to the condition.

## Objective
To gain insights into diabetes patterns among the Pima Indians tribe and build a robust predictive model to support informed healthcare decision-making.

## Dataset
The dataset includes the following features:
- **Pregnancies**: Number of pregnancies
- **Glucose**: Plasma glucose concentration after a 2-hour oral glucose tolerance test
- **Blood Pressure**: Diastolic blood pressure (mm Hg)
- **Skin Thickness**: Triceps skinfold thickness (mm)
- **Insulin**: 2-hour serum insulin (mu U/ml)
- **BMI**: Body mass index (kg/(m²))
- **Diabetes Pedigree Function**: Likelihood of diabetes based on family history
- **Age**: Age in years
- **Outcome**: Diabetes class variable (0: non-diabetic, 1: diabetic)

## Methodology
The project employed a structured analytical approach:

1. **Data Exploration & Quality Assessment**
   - Conducted initial statistical analysis to understand data distributions
   - Identified missing values using visualization techniques
   - Detected and managed outliers through IQR method and domain knowledge

2. **Feature Engineering & Selection**
   - Created derived metrics from existing features to enhance predictive power
   - Applied correlation analysis to identify significant predictors
   - Used SelectKBest with chi-squared test to determine feature importance

3. **Modeling Approach**
   - Implemented multiple classification algorithms (Logistic Regression, Random Forest, SVM)
   - Used stratified k-fold cross-validation to ensure model reliability
   - Applied hyperparameter tuning through grid search for optimal model performance

4. **Evaluation Strategy**
   - Assessed models using balanced metrics (accuracy, precision, recall, F1-score)
   - Created confusion matrices to understand error patterns
   - Implemented ROC-AUC analysis to evaluate model discrimination ability

## Workflow
1. **Data Loading & Cleaning**
   - Import the dataset
   - Handle missing values and outliers
2. **Exploratory Data Analysis (EDA)**
   - Visualize variable distributions and relationships
   - Identify trends and correlations
3. **Data Preprocessing**
   - Standardize/normalize numerical features
   - Split the dataset into training and testing sets
4. **Model Training**
   - Train a classification model (e.g., Logistic Regression, Random Forest)
   - Evaluate with metrics such as accuracy, precision, and recall
5. **Interpretation & Recommendations**
   - Analyze key features influencing predictions
   - Provide actionable insights for diabetes prediction

## Results and Observations
The analysis revealed several significant patterns in diabetes prevalence:

- Glucose levels demonstrated the strongest correlation with diabetes diagnosis, with readings above 140 mg/dL showing particularly high risk
- BMI emerged as the second most significant predictor, with values above 30 associated with increased diabetes likelihood
- Age and number of pregnancies showed moderate correlation with diabetes outcomes
- The final Random Forest model achieved 78% accuracy with balanced precision and recall, outperforming other algorithms tested
- Feature importance analysis confirmed clinical understanding that glucose regulation, BMI, and family history (diabetes pedigree function) are critical indicators

## Future Work
- Expand the dataset with additional health metrics and lifestyle factors
- Implement more advanced ensemble methods and deep learning approaches
- Develop a risk stratification system for early intervention
- Validate the model on diverse populations to test generalizability

Happy Analyzing!
