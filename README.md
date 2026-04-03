# 💎 Diamond Price Prediction & Market Analysis using Regression Modeling

## Problem
Diamond pricing is influenced by multiple factors beyond the traditional “4Cs” (Carat, Cut, Color, Clarity), including market dynamics, certification, and consumer perception. Unlike commodities like gold, diamond valuation is complex and often inconsistent.

This project aims to:
- Identify key factors influencing diamond prices  
- Analyze pricing patterns and potential market inefficiencies  
- Build regression models to explain and predict diamond pricing  


## Solution
Developed a comprehensive regression modeling pipeline combining statistical techniques and machine learning to analyze diamond pricing. The project evaluates multiple models, applies feature selection techniques, and performs residual analysis to ensure robustness and interpretability.


## Key Features
- Extensive **Exploratory Data Analysis (EDA)** with visual insights  
- **Data cleaning & preprocessing** (handling missing values, encoding)  
- **Feature selection using VIF analysis** to reduce multicollinearity  
- **Stepwise regression (forward & backward selection)**  
- **Feature transformation** (log, square, exponential) to handle skewness  
- **Model comparison** (baseline, first-order, interaction models)  
- **Residual analysis** for model validation  
- **LASSO regression** for feature regularization  
- Business-driven interpretation of results  


## Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Statsmodels  
- Scikit-learn  


## Models & Methodology

### 1. Baseline Model
- Used log-transformed carat weight  
- Adj R²: ~0.17  
👉 Established baseline for comparison  

### 2. First-Order Regression Model
- Included all selected features  
- Adj R²: ~0.65  
👉 Best predictive performance  

### 3. Interaction Model
- Focused on interactions between key variables (Cut, Color, Clarity, Carat)  
- Adj R²: ~0.55  
👉 Improved interpretability of relationships  

### 4. LASSO Regression
- Used for feature selection and regularization  
- Confirmed relevance of selected predictors  


## Results & Insights
- **Carat Weight** is the strongest predictor of price (positive correlation)  
- **Lab-grown diamonds** significantly reduce price  
- **Clarity (IF, VVS1, VVS2)** positively impacts price  
- **Color G diamonds** showed higher prices than colorless (D) → suggests market inefficiency  
- **Shape and Cut interactions** influence pricing in non-linear ways  
- Evidence of **pricing inconsistencies for identical diamonds**, indicating market inefficiencies  


## Model Performance (Train/Test)

| Model            | R² (Test) | RMSE |
|------------------|----------|------|
| First-order      | ~0.70    | ~0.28 |
| Interaction      | ~0.57    | ~0.34 |

👉 First-order model performed better in prediction
👉 Interaction model provided better interpretability  


## Key Learnings
- Feature engineering and transformation significantly improve model performance  
- Multicollinearity must be handled carefully (VIF analysis critical)  
- Simpler models can outperform complex ones in prediction  
- Statistical interpretation is as important as predictive accuracy  


## Future Improvements
- Incorporate time-based data to analyze market trends  
- Include additional features (e.g., certification, seasonal demand)  
- Deploy as an interactive pricing tool  
- Explore advanced ML models (XGBoost, ensemble methods)
- 

## Dataset
- Sourced from Kaggle (Diamond Pricing Dataset)

