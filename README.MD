# 💰 Insurance Charges Analysis

This project investigates how **demographic and socio-economic factors** affect individual health insurance charges. The analysis focuses on the predictive power of features like age, BMI, smoking status, and number of children in determining insurance premiums.

---

## 🎯 Objective

To determine which variables most strongly influence health insurance charges and assess how well these factors predict costs.  
This analysis is valuable for:
- Individuals seeking to understand their premiums
- Insurers modeling risk
- Policymakers promoting affordability

---

## 📂 Dataset

- The dataset includes variables such as:
  - `age`
  - `sex`
  - `bmi`
  - `children`
  - `smoker`
  - `region`
  - `charges` (target variable)

---

## 🧪 Methodology

### 🔹 Data Exploration
- Used `ggpairs()` and summary statistics for quick overview
- Plotted distributions for BMI, age, and charges
- Examined charges across regions and smoking status

### 🔹 Correlation Analysis
- Built correlation matrix using `corrplot`
- Identified strong correlations between smoking and charges

### 🔹 Statistical Modeling
- Fitted multiple linear regression models
- Performed model comparison with and without smoking status
- Included interaction terms (e.g., BMI × smoker) to assess combined effects

### 🔹 Model Evaluation
- Used R², adjusted R², and p-values
- Interpreted coefficients to understand marginal effects
- Validated model assumptions via residual plots

---

## 📊 Key Findings

- **Smoking status** has the most significant impact on insurance charges  
- **BMI** and **age** are also positively correlated with higher premiums  
- Interaction between **BMI and smoking** magnifies cost  
- **Gender** and **region** have minimal predictive power in this context

---

## 📦 Tools & Libraries

This project is built using **R** and **Quarto** with the following libraries:

```r
tidyverse    # Data wrangling and visualization
knitr        # Report formatting
corrplot     # Correlation heatmaps
gridExtra    # Arranging multiple plots
GGally       # Advanced pairwise plots
```