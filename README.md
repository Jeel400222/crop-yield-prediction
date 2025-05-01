
# 🌾 Crop Yield Prediction

This project focuses on building a regression-based machine learning model to predict crop yield based on soil nutrients (Nitrogen, Phosphorus, Potassium) and environmental conditions (temperature, humidity, pH, rainfall). The model helps farmers and agricultural planners make informed decisions to optimize crop production.

---

## 📌 Problem Statement

Accurately predicting crop yield is essential for food security and resource management. Traditional methods often rely on historical trends without considering changing climate and soil conditions. This project leverages machine learning to provide dynamic and data-driven yield predictions.

---

## 📊 Dataset Overview

- **Source**: [Crop_recommendation.csv] (synthetic yield column added)
- **Features**:
  - Nitrogen (N)
  - Phosphorus (P)
  - Potassium (K)
  - Temperature (°C)
  - Humidity (%)
  - pH
  - Rainfall (mm)
- **Target**:
  - Synthetic `Yield` (tons/hectare)

---

## 🔍 Exploratory Data Analysis (EDA)

- Analyzed distributions, correlations, and missing values
- Identified Rainfall and Nitrogen as the most influential features
- Visualized feature importance using Random Forest Regressor

---

## 🧹 Data Preprocessing

- Handled missing values
- Scaled numerical features
- Performed one-hot encoding (if needed)
- Split data into training and test sets

---

## 🧠 Modeling & Performance

| Model               | R² Score | RMSE   | Cross-Validation R² |
|--------------------|----------|--------|----------------------|
| Random Forest       | 0.9942   | 0.0155 | 0.9930 ± 0.0011      |
| Linear Regression   | 0.6977   | 0.5653 | Not used             |

> 🎯 **Random Forest Regressor** clearly outperformed others in predictive accuracy.

---

## 📈 Interactive Prediction

A custom input form allows users to input soil and weather data:
```
Example:
Nitrogen (N): 33
Phosphorus (P): 21
Potassium (K): 25
Temperature (°C): 29
Humidity (%): 65
pH: 4
Rainfall (mm): 77
```
🔮 **Predicted Yield:** `0.38 tons/hectare`

---

## 🛠 Tech Stack

- Python
- Jupyter Notebook
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- RandomForestRegressor, LinearRegression
- Git/GitHub for version control

---

## 📝 Executive Summary

See [executive_summary.md](executive_summary.md) for a 1–2 page project summary with objective, key metrics, and findings.

---

## 🔮 Future Improvements

- Use real-world yield datasets for better generalization
- Try advanced models like XGBoost or deep learning
- Integrate live weather APIs
- Add outlier detection and noise handling

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙌 Acknowledgments

- Inspired by agricultural research and precision farming efforts
- Dataset adapted from `Crop_recommendation.csv`

---

## 🤝 Contributing

Feel free to fork this repository, raise issues, or submit pull requests!
