# Employee Salary Prediction

## Project Overview
Predict employee salary using demographic and job-related features.

## Dataset
Features:
- Age
- Experience
- Education
- Department
- Location

Target:
- Salary

## EDA
Key findings:
- Experience strongly correlated with Salary (0.86)
- Age had weaker correlation (0.10)
- No missing values

## Preprocessing
- StandardScaler for numeric features
- OneHotEncoder for categorical features
- ColumnTransformer
- Pipeline

## Models
### Linear Regression
R² = 0.7778

### Linear Regression (All Features)
R² = 0.9429

### Ridge Regression + GridSearchCV
R² = 0.9428

## Cross Validation
Mean R² = 0.9396
Std = 0.0066

## Conclusion
Education significantly improved model performance.
The final model explained over 94% of salary variation.

## Future Improvements
- Use real salary data
- Try XGBoost
- Deploy with Streamlit
## 
new_employee = pd.DataFrame ({
    "Age": [30],
    "Experience": [5],
    "Education": ["Master"],
    "Department": ["IT"],
    "Location": ["Dhaka"]
})

best_model.predict(new_employee)
