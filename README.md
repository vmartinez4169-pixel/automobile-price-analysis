# Automobile-Price-Analysis
Phase 2 Capstone Project - Automobile Price Analysis and Prediction

# Final Analysis Report: Automobile Price Prediction

## Executive Summary
This project analyzes key physical and mechanical attributes of vehicles to build a predictive model for automobile pricing. The final linear model provides non-technical stakeholders with a data-driven tool to estimate market value based on core vehicle specifications.

## 1. Exploratory Data Analysis (EDA)
* Identified strong linear relationships between vehicle price and key mechanical metrics (`engine-size`, `curb-weight`, and `horsepower`).
* Discovered significant price variation across categorical attributes—Rear-Wheel Drive (`rwd`) vehicles command higher median prices than Front-Wheel Drive (`fwd`) models.
* Uncovered missing data sentinels (`?`) and target row gaps.

## 2. Preprocessing & Data Cleaning
* **Target Treatment:** Dropped rows missing target variable values (`price`) to prevent modeling bias.
* **Imputation:** Applied median imputation for continuous variables and mode imputation for categorical attributes.
* **Encoding:** Applied One-Hot Encoding (`pd.get_dummies` with `drop_first=True`) to convert categories like `drive-wheels` and `body-style` into numerical inputs while avoiding multicollinearity.

## 3. Modeling & Performance
* Fitted an Ordinary Least Squares (OLS) Linear Regression model on an 80/20 train-test split.
* Evaluated model accuracy using MAE, RMSE, and $R^2$ score on unseen test data.
* Interpreted feature coefficients to determine top positive drivers (e.g., engine displacement and performance build).

## 4. Dashboard Insights
The accompanying Tableau Public dashboard allows non-technical team members to interactively explore price distributions across vehicle makes, body styles, and performance tiers. 
* **Tableau Public Link:** [Insert Your Tableau Public URL Here]
