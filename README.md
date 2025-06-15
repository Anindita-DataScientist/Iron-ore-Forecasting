Iron Ore Price Forecasting Using Machine Learning 📈-This project aims to forecast Iron Ore Prices enabling industries to make smarter procurement and inventory decisions by minimizing price volatility risks.

✅ Objective- Forecast future iron ore prices using machine learning.Help steel and manufacturing sectors reduce procurement costs and predict market trends.Build a user-friendly tool for interactive prediction and visualization.

🧰 Tech Stack & Tools

🖥 Programming Language:
Python 3.9

🔍 Libraries & Frameworks:
Data Manipulation: Pandas, NumPy

Visualization: Matplotlib, Seaborn, Plotly

Modeling & Evaluation: Scikit-learn, Random Forest Regressor

Deployment: Streamlit

Environment: Jupyter Notebook, Spyder

🔄 Step-by-Step Workflow

1. 📥 Data Collection
Collected historical iron ore price data (.csv).
Included monthly price data over multiple years.

2. 📊 Exploratory Data Analysis (EDA)
Checked for:
Missing values
Outliers
Seasonality and trends
Visualizations used:
Line plots for trend detection
Correlation heatmaps
Box plots to detect volatility

3. 🧼 Data Preprocessing
Converted date column to datetime type.

Extracted month, year, and lag features.

Filled missing values using interpolation.

Removed extreme outliers based on domain logic.

Created moving averages (3-month, 6-month).

Feature scaling using StandardScaler.

4. 🧠 Model Building: Random Forest
Used Random Forest Regressor as the final model.

Reason for choosing:

Handles non-linearity well

Robust against overfitting

Works well with time-dependent engineered features

5. 📊 Model Evaluation
Evaluation metrics:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

R² Score

Observations:

Random Forest outperformed baseline models like Linear Regression.

Residual plots showed no significant bias.

6. 🔧 Hyperparameter Tuning
Performed tuning using GridSearchCV

Tuned parameters:

n_estimators (number of trees)

max_depth

min_samples_split

min_samples_leaf

Selected best parameters based on cross-validated RMSE.

7. 📦 Deployment Using Streamlit
Created a Streamlit app to:

Upload custom CSV

Visualize data trends

Predict iron ore prices

Display forecast plots with confidence zones

Deployed locally and tested for production-readiness.

🧠 Key Achievements & Insights
Final model: ✅ Random Forest Regressor

Achieved an R² score above 0.85 with low MAE and RMSE.

Discovered:

Seasonal spikes in iron ore prices due to global demand cycles.

Lag-based features significantly improved accuracy.

📌 Streamlit App Features

📂 Upload historical CSV file

📈 View interactive trend graphs

📊 Show predictions with price bands

📄 Simple sidebar-based input and forecasting options

