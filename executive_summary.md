
# 🌾 Executive Summary: Crop Yield Prediction

## 🎯 Project Objective
To predict crop yield using key environmental and soil nutrient data, empowering farmers with data-driven insights for crop planning. The model is trained on an extended version of the Crop Recommendation dataset, including synthetic yield values.

## 📊 Key Findings
- **Best Model:** Random Forest Regressor  
- **Root Mean Squared Error (RMSE):** 0.0155  
- **R² Score:** 0.9942  
- **Cross-Validation R²:** 0.9930 ± 0.0011  
- **Top Influential Features:** Rainfall and Nitrogen  

## 🧪 Methodology Summary
- Conducted EDA and preprocessing on the dataset (handling nulls, encoding).
- Engineered a synthetic target variable (yield) to simulate real-world outputs.
- Compared multiple models — Random Forest outperformed Linear Regression.
- Performed k-fold cross-validation and feature importance analysis.
- Built an interactive prediction UI using Python (input: N, P, K, pH, etc.).

### 📍 Sample Prediction
> **Inputs:** N=33, P=21, K=25, Temp=29°C, Humidity=65%, pH=4, Rainfall=77mm  
> **Predicted Yield:** **0.38 tons/hectare**

## ✅ Final Recommendations
- Incorporate **real-world yield datasets** to replace synthetic labels.
- Add models like **XGBoost**, **LSTM**, or **CNNs** for complex patterns.
- Use **real-time weather APIs** to automate input collection.
- Deploy the model as a **web app** using Streamlit for farmers and agronomists.

## 🛠️ Tools & Tech Stack
- Python (pandas, scikit-learn, matplotlib, seaborn)
- Jupyter Notebook
- Streamlit (for future UI)
- Git & GitHub
