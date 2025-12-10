This repository provides an end-to-end framework for inventory demand forecasting in small retail stores. The focus is on predicting daily sales accurately while keeping the models transparent and usable for real business environments.

The project includes:

• 11 forecasting models, evaluated under the same experimental conditions
• A consistent preprocessing pipeline with lag features, rolling statistics, encoding and scaling
• Chronological train–test splitting to respect time-dependency
• Comparison using MAE, RMSE, MAPE/sMAPE and R²
• Exported results: predictions, metrics, trained models and plots
• SHAP explainability for model transparency
• A lightweight dashboard to explore forecasts and errors

The 11 models are:

• Linear Regression
• Ridge Regression
• Lasso Regression
• Elastic Net Regression
• Decision Tree Regressor
• Random Forest Regressor
• XGBoost
• LightGBM
• CatBoost
• Support Vector Regression
• k-Nearest Neighbour

The dataset contains ~73,000 daily records across multiple stores and products, including:

• sales quantity
• pricing
• promotions
• holidays
• weather effects
• competitor influence

All models follow a common workflow:

• Data cleaning and transformation
• Feature engineering and lag creation
• Model training
• Metric evaluation
• Visual analysis
• Artifact export

Results include:

• Bar charts for MAE/RMSE
• Radar charts for top models
• Time-series overlays for actual vs predicted values
• Feature importance and SHAP plots
• A ranking table from best to lowest performance

Deployment options include:

• Flask or Streamlit apps
• Excel or Power BI dashboards
• Local execution on standard laptops (no GPU required)

The framework is designed for small retail shops that want:

• better stock planning
• fewer stockouts
• reduced waste
• clearer insights
• fast and lightweight forecasting tools

By comparing 11 models, the project shows which approaches offer the best balance between accuracy and interpretability, making inventory forecasting both practical and explainable for non-technical users.
