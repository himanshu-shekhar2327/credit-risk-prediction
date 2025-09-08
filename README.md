# German Credit Risk Prediction  

This project predicts **credit risk** (Good vs Bad) using the **German Credit Dataset** from Kaggle.  
The goal is to explore end-to-end machine learning workflow: data preprocessing, visualization, model training, hyperparameter tuning, and evaluation.  

---

## 📊 Dataset  
- Source: Kaggle – German Credit Dataset  
- Features: 8 selected features including Age, Sex, Job, Housing, Saving accounts, Checking account, Credit amount, Duration.  
- Target: Credit Risk (0 = Bad, 1 = Good).  

---

## ⚙️ Workflow  
1. **Data Exploration & Cleaning**  
   - Handled missing values (dropped rows with nulls).  
   - Explored dataset with `describe()`, `info()`, and shape checks.  
   - Visualized data using box plots, violin plots, scatter plots, heatmaps, and count plots.  

2. **Feature Engineering**  
   - Label encoding applied to categorical columns (`Sex`, `Housing`, `Saving accounts`, `Checking account`).  
   - Stored encoders with `joblib` for consistent transformations.  

3. **Model Training & Tuning**  
   - Tried multiple models:  
     - Decision Tree  
     - Random Forest  
     - Extra Trees  
     - XGBoost  
   - Applied **GridSearchCV** for hyperparameter tuning.  

4. **Evaluation**  
   - Compared accuracy, precision, recall, F1-score.  
   - Best model: **XGBoost** with ~68% accuracy.  
   - Confusion Matrix used to analyze predictions.  

5. **Model Saving**  
   - Final trained XGBoost model saved with `joblib` → `best_xgb.pkl`.  
   - Encoders saved separately for deployment.  

---

## 🚀 Tech Stack  
- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn, Joblib  
- **Tools:** Jupyter Notebook  

---

## 📈 Results  
- **Best Model:** XGBoost  
- **Final Accuracy:** ~68%  
- **Key Insight:** Credit risk prediction is highly dependent on account details (`Saving accounts`, `Checking accounts`) and loan amount/duration.  

---

## 🔮 Future Improvements  
- Handle missing values with imputation instead of dropping.  
- Balance dataset (if imbalanced) using SMOTE or class weights.  
- Deploy model with **Streamlit/Flask** for interactive use.  
- Experiment with deep learning models.  

---

## 👨‍💻 Author  
- **Himanshu Shekhar** – Enthusiast Data Scientist and ML Engineer 
- 📧 Contact: [himanshu.shekhar0505@gmail.com]  
- 🌐 Portfolio: [your-portfolio-link]  
