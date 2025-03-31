# Impact-of-Repo-Rate-and-ROA-on-Debt-Equity-Ratio

# 📊 Debt-Equity Ratio Analysis using Multiple Linear Regression

This repository contains the full analysis pipeline for understanding how macroeconomic variables like **Repo Rate** and **Return on Assets (ROA)** influence the **Debt-Equity Ratio** of companies in **India** and **South Africa**.

---

## 🧠 Objective

- To model and evaluate how **ROA** and **Repo Rate** affect a company’s **Debt-Equity Ratio**.
- Compare the strength of this relationship between companies based in **India** and **South Africa**.
- Perform regression diagnostics to assess the robustness of the model.

---

## 📂 Dataset

Two datasets used:
- `India Company.xlsx`
- `SA Company.xlsx`

Each dataset contains:
- `YEAR`
- `COMPANY`
- `REPO RATE`
- `ROA`
- `DEBT EQUITY`

---

## 🧪 Methods Applied

1. **Exploratory Data Analysis (EDA)**
   - Pairplots to explore correlations
   - Histograms to inspect skewness

2. **Multiple Linear Regression**
   - Dependent Variable: `DEBT EQUITY`
   - Independent Variables: `REPO RATE`, `ROA`

3. **Statistical Tests & Diagnostics**
   - p-values for significance testing
   - Variance Inflation Factor (VIF) for multicollinearity
   - Durbin-Watson test for autocorrelation
   - Breusch-Pagan test for heteroskedasticity
   - Residual plots for model assumptions

---

## 📈 Final Results Summary

| Aspect                  | India                         | South Africa                    |
|-------------------------|-------------------------------|----------------------------------|
| R² (Explanatory Power)  | 12.6% (low)                   | 1.8% (very poor)                |
| Significant Predictor   | ROA (**strong negative**)     | ROA (**moderate negative**)     |
| Repo Rate               | Marginally significant        | Not significant                 |
| Multicollinearity       | Not present                   | Not present                     |
| Autocorrelation         | Present (**DW < 1**)          | Present (**DW < 1**)            |
| Heteroskedasticity      | Present (**p < 0.001**)       | Not Present (**p > 0.05**)      |

---

## 🛠️ Requirements

Make sure the following Python libraries are installed:

```bash
pip install -r requirements.txt
```
