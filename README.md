# Crop-Yield-Prediction
Using two ML models-Gradient Boosting,Random Forest

# 🌾 Crop Yield Prediction using Machine Learning

This project focuses on predicting crop yields using machine learning techniques. It utilizes data preprocessing, feature engineering, and model training to develop a robust predictive model. The goal is to help farmers and agricultural planners estimate crop yield more accurately, supporting better decision-making and resource management.

---

## 🧪 Project Workflow

### 1. 📥 Data Handling
- Load the crop dataset (`dmt-dataset.csv`)
- Handle missing values in numerical and categorical columns
- Drop non-essential columns like `Date`
- Encode categorical values such as `Location` and `Crop Type`

### 2. 🔬 Feature Engineering
- Use `StandardScaler` for normalization
- Apply `SelectKBest` for feature selection
- Generate polynomial features using `PolynomialFeatures` to capture non-linear interactions

### 3. 📊 Model Building
- Split dataset into train and test sets (80/20)
- Use **XGBoost Regressor** (`xgb.XGBRegressor`) for predictive modeling
- Train on polynomial-enhanced features

### 4. 📈 Evaluation
- Evaluate model performance using:
  - **Mean Squared Error (MSE)**
  - **R² Score**
- Visualize prediction results using:
  - Heatmaps (correlation matrix)
  - Yield distribution histogram
  - Scatter plot of actual vs predicted yields

---

## 📦 Requirements

```bash
pip install pandas numpy xgboost scikit-learn matplotlib seaborn
```

---

## 🚀 How to Run

1. Place your dataset file (`dmt-dataset.csv`) in the same directory as your notebook/script.
2. Run the Jupyter Notebook: `Crop-Yield-PredictionFinal.ipynb`
3. Visualizations and evaluation metrics will be displayed at the end of the notebook.

---

## 🧠 Technologies Used

- Python
- Jupyter Notebook
- XGBoost
- Scikit-learn
- Matplotlib & Seaborn

---

## 📊 Results Snapshot

- **Model Used:** XGBoost Regressor
- **Key Metrics:** MSE, R² Score
- **Feature Scaling & Selection:** Standardization + SelectKBest
- **Visualizations:** Heatmap, Histogram, Actual vs Predicted Scatter

---

## 📁 Dataset Overview

The dataset (`dmt-dataset.csv`) includes:
- Input features: Weather conditions, soil quality, crop type, location, etc.
- Output variable: Crop yield (numerical)

---

## 🤝 Acknowledgments

- Dataset: Prepared and cleaned using publicly available agricultural data
- Tools: [XGBoost](https://xgboost.readthedocs.io/), [scikit-learn](https://scikit-learn.org/), [Matplotlib](https://matplotlib.org/)

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 👨‍💻 Authors

- Krishna Sai (21MIS0109)  
- Kishore M (21MIS0314)  
- Mohan Balaji B (21MIS0434)
