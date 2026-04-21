# 📊 Income Prediction with Machine Learning

<p align="center">
  <img alt="Python" src="https://img.shields.io/badge/Python-3.x-blue?logo=python">
  <img alt="Scikit-learn" src="https://img.shields.io/badge/Scikit--learn-ML-orange?logo=scikitlearn">
  <img alt="Pandas" src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas">
  <img alt="NumPy" src="https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy">
  <img alt="Matplotlib" src="https://img.shields.io/badge/Matplotlib-Visualization-blue">
  <img alt="Status" src="https://img.shields.io/badge/Status-Completed-success">
</p>

## 🎯 Objective
This project aims to predict customer income based on demographic, financial, and behavioral features using Machine Learning techniques.

## ⚙️ Project Workflow

### 1. Data Preprocessing
- Handling missing values
- Encoding categorical variables with `get_dummies`
- Aligning train and test datasets
- Converting features to numeric format

### 2. Models Evaluated
- Ridge Regression
- Lasso Regression
- Stepwise Selection
- Random Forest
- Random Forest (GridSearchCV) 

### 3. Final Model
The best-performing model was:

```python
RandomForestRegressor (optimized with GridSearchCV)
```

| Model                            |       R² |           RMSE |
| -------------------------------- | -------: | -------------: |
| Ridge / Lasso                    |     0.26 |          ~7019 |
| Stepwise                         |     0.24 |          ~7139 |
| Gradient Boosting                |     0.39 |          ~6378 |
| Random Forest                    |    ~0.41 |          ~6300 |
| **Random Forest (GridSearchCV)** | **0.42** | **~6200–6300** |

## 📈 Model Evaluation Dashboard

The dashboard below summarizes the final model performance, including feature importance, prediction accuracy, residual analysis, and error distribution.

<img width="1389" height="990" alt="Image" src="https://github.com/user-attachments/assets/76724fdd-3879-4a15-8812-dac4601a958e" />

---

## 🔍 Key Findings

- The tuned Random Forest outperformed linear models and better captured non-linear relationships in income prediction.
- The model performed well for low and medium income ranges, where most observations are concentrated.
- High-income values were more difficult to predict and tended to be underestimated.
- Employment duration was the most important variable in the final model.

## 💡 Final Insight

The model achieved solid performance (R² ≈ 0.42), accurately predicting low and medium income ranges where most observations are concentrated.  
However, residual analysis shows systematic underestimation of high-income values and the presence of heteroscedasticity, indicating increasing prediction uncertainty at higher income levels.  
Despite these limitations, the model provides valuable insights—especially the importance of employment duration—and can be improved through target transformation, outlier treatment, and enhanced feature engineering.

## ⚠️ Limitations

- Moderate explanatory power  
- Difficulty predicting high-income observations  
- Presence of heteroscedasticity  
- Sensitivity to outliers  


## 🚀 Next Steps
 
- Improve feature engineering  
- Handle outliers more effectively  


## 🛠️ Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  
- Statsmodels

## ✅ Conclusion

The Random Forest model optimized with GridSearchCV proved to be the most effective approach, outperforming linear models and capturing non-linear relationships in customer income.  
This result highlights the importance of non-linear patterns in the data, which were better modeled by tree-based methods.  
Despite solid performance, further improvements can be achieved through feature engineering, outlier handling, and more advanced algorithms.

## 👤 Author

**Karolainy de sousa arantes**  
[LinkedIn](https://www.linkedin.com/in/karolainy-de-sousa-arantes-560801303/) 
