# 🥦 Vegetable Price Analysis – Capstone Project

## 📌 Project Overview

This project aims to analyze and predict daily vegetable prices in India using historical data from January 1, 2023 to January 1, 2024. The primary goal is to forecast **Tomato prices** based on the prices of other vegetables, providing actionable insights for stakeholders such as farmers, retailers, and policymakers.

This project was completed as part of the **Explore AI Academy Capstone**, emphasizing real-world data science applications in agriculture.

## 📊 Dataset Description

- **Source**: AGMARKNET, Kaggle Vegetable Price Datasets  
- **Format**: CSV  
- **Time Span**: 366 daily entries (Jan 2023 – Jan 2024)  
- **Vegetables Included**: Tomato, Onion, Potato, Bhindi, Brinjal, Garlic, Peas, Methi, Green Chilli, Elephant Yam  
- **Structure**: Each row represents a day with corresponding prices for each vegetable.

## ⚙️ Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/veengramoney/vegetable-price-analysis.git
   ```
2. Navigate to the project folder:
   ```bash
   cd vegetable-price-analysis
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Vegetable_Price_Analysis.ipynb
   ```

## 🧪 Methodology

### 🔹 Data Cleaning
- Removed missing values  
- Standardized date formats  
- Normalized price units (e.g., per kg)  
- Flagged and removed outliers  
- Saved cleaned dataset for modeling

### 🔹 Exploratory Data Analysis (EDA)
- Histograms and box plots for distribution  
- Scatter plots for pairwise relationships  
- Correlation matrix to assess linear dependencies  
- Insights on volatility and seasonal trends

### 🔹 Modeling
- Models used:
  - Linear Regression  
  - Random Forest Regressor  
  - Gradient Boosting Regressor  
- Feature scaling applied  
- Train/test split (80/20)  
- Evaluation using RMSE and R²  
- Cross-validation for stability

## 📈 Key Insights

- Tomato prices show high volatility and weak linear correlation with other vegetables  
- Ensemble models outperform linear models  
- Feature scaling significantly improves model performance  
- Random Forest achieved perfect test results (possible overfitting)

## 📊 Evaluation Metrics

ModelRMSER² ScoreLinear Regression0.170.0000| Random Forest      | 0.00  | 1.0000   |
| Gradient Boosting  | 0.00  | 0.0000   |

## 📌 Conclusion

- Random Forest was selected as the final model due to its ability to capture non-linear relationships.
- The project demonstrates the importance of robust preprocessing and model selection in agricultural forecasting.
- Overfitting concerns suggest the need for external validation and additional features.

## 🚀 Future Work

- Integrate external data (e.g., weather, fuel prices, demand)  
- Explore time series models (ARIMA, Prophet)  
- Apply hyperparameter tuning (GridSearchCV)  
- Improve notebook structure and Markdown clarity  
- Enhance visualizations and storytelling for stakeholders

## 📁 Project Structure

```
vegetable-price-analysis/
│
├── data/
│   ├── prices.csv
│   └── cleaned_prices.csv
│
├── notebooks/
│   └── Vegetable_Price_Analysis.ipynb
│
├── visuals/
│   └── plots/
│
├── README.md
└── requirements.txt
```

## 🙌 Acknowledgments

- Project Lead: **Neville Gramoney**  
- Technical Support: **Copilot AI Assistant**  
- Institution: **Explore AI Academy**  
- Special thanks to mentors and reviewers for feedback and guidance.
