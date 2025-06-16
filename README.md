📈 Iron Ore Price Forecasting Using Machine Learning
This project aims to forecast Iron Ore Prices to help industries make smarter procurement and inventory decisions, ultimately reducing the impact of price volatility in the steel and manufacturing sectors.

## 🎯 Objective
Forecast future iron ore prices using machine learning.

Help steel and manufacturing sectors reduce procurement costs and predict market trends.

Build a user-friendly tool for interactive forecasting and data visualization.

## 🧰 Tech Stack & Tools
### 🖥 Programming Language
Python 3.9

## 🔍 Libraries & Frameworks
Data Manipulation- Pandas,NumPy

Visualization- Matplotlib, Seaborn, Plotly

Modeling & Evaluation- Scikit-learn, Random Forest Regressor

Deployment- Streamlit

Development Environment- Spyder

## 🔄 Step-by-Step Workflow
### 1. 📥 Data Collection
Collected historical iron ore price data (.csv format).

Included monthly price data spanning several years.

### 2. 📊 Exploratory Data Analysis (EDA)
Goals:

Detect missing values and outliers

Identify seasonality and long-term trends

Tools Used:

Line plots → To analyze price trends over time

Correlation heatmaps → To understand feature relationships

Box plots → To detect price volatility and distribution

### 3. 🧼 Data Preprocessing
Steps Performed:

Converted Date column to datetime type

Extracted:

Month

Year

Lag features (e.g., previous month prices)

Filled missing values using linear interpolation

Removed extreme outliers using domain-specific logic

Created moving average features (3-month, 6-month)

Scaled numerical features using StandardScaler

### 4. 🧠 Model Building – Random Forest Regressor
Model Chosen: ✅ Random Forest Regressor
Reason:

Handles non-linear relationships

Resistant to overfitting

Works well with time-series engineered features

Baseline models like Linear Regression were tested but underperformed.

### 5. 📊 Model Evaluation
Metrics Used:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

R² Score

Results:

Achieved R² > 0.85

Residual plots indicated no significant bias

### 6. 🔧 Hyperparameter Tuning
Used GridSearchCV to find optimal parameters:

n_estimators – Number of trees

max_depth – Maximum depth of each tree

min_samples_split – Minimum samples to split an internal node

min_samples_leaf – Minimum samples per leaf

Best parameters were selected based on cross-validated RMSE.

### 7. 📦 Deployment Using Streamlit
Developed a clean Streamlit interface to:

📂 Upload custom CSV datasets

📈 Visualize historical trends

📊 Predict future iron ore prices

📉 Show forecast plots with confidence bands

Status:
✅ Deployed locally and tested for production-readiness

## 🌟 Key Achievements & Insights
✅ Final Model: Random Forest Regressor

✅ Achieved R² > 0.85, with low MAE and RMSE

✅ Key Findings:

Seasonal patterns tied to global demand cycles

Lag-based and rolling average features improved model performance

## 📌 Streamlit App Features
📂 Upload historical .csv files

📈 Interactive trend and forecast graphs

📊 Forecasted price with confidence zones

🔧 Simple sidebar-based input for quick testing













