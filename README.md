# Graduate Admission Prediction

This project develops and evaluates machine learning models to predict a graduate applicant’s **Chance of Admit** based on profile features such as GRE, TOEFL, CGPA, University Rating, SOP, LOR, and Research experience.  
The notebook walks through a **complete data analysis pipeline**: from problem definition and exploratory data analysis to modeling, evaluation, interpretability, and conclusions.

---

## 📌 Problem Statement
Universities receive thousands of applications every year. Manually evaluating each profile is time-consuming and subjective.  
**Can we use applicant data to predict admission probability and identify the most important factors influencing decisions?**

---

## 🎯 Goals
- Build a predictive model for **Chance of Admit**.  
- Identify which features most strongly impact admission chances.  
- Provide interpretable insights for applicants and universities.  

---

## ❓ Key Questions
1. Which applicant attributes correlate most strongly with admissions?  
2. Does research experience significantly increase the chance of admission?  
3. How well can machine learning models predict the target?  
4. Which model type (linear, tree-based, ensemble, etc.) performs best?  

---

## 📊 Methodology
1. **Data Audit & Cleaning**  
   - Standardized column names, removed index columns, checked duplicates & missing values.  

2. **Exploratory Data Analysis (EDA)**  
   - Distributions of all numeric features  
   - Correlation matrix & scatterplots with trendlines  
   - Boxplots of Chance of Admit by Research and University Rating  

3. **Modeling & Evaluation**  
   - Baseline (mean predictor)  
   - Linear Regression, Ridge, Lasso, ElasticNet  
   - Random Forest, Gradient Boosting  
   - 5-fold cross-validated **GridSearchCV**  
   - Metrics: RMSE, MAE, R²  

4. **Diagnostics & Interpretability**  
   - Residual analysis, predicted vs actual plots  
   - Permutation Feature Importance  
   - Partial Dependence Curves for top features  

5. **Conclusions & Recommendations**  
   - Insights for both **students** (how to strengthen applications) and **universities** (screening aid).  

---

## 📈 Results
- **Top drivers of admission probability**: CGPA (strongest), GRE, TOEFL, then University Rating, SOP, LOR, and Research.  
- **Best models**: Gradient Boosting and Random Forest, achieving the lowest RMSE and highest R² on test data.  
- **Research experience** provides a consistent positive boost to admit probability.  

---

## 💡 Conclusions
- Academic performance (CGPA, GRE, TOEFL) remains the most decisive factor in admissions.  
- Soft factors (SOP, LOR) and Research contribute but less strongly.  
- Ensemble models significantly outperform simple baselines, showing the value of machine learning.  
- The model can serve as a **screening aid**, but final decisions require holistic evaluation.  

---
