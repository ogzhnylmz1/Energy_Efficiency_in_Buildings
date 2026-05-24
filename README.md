# Energy Efficiency in Buildings
Energy Efficiency Optimization and Predictive Modeling in Buildings Using Multiple Linear Regression in SPSS.

# Energy Efficiency & Predictive Modeling: Building Heating Load Analysis

This project develops a **Multiple Linear Regression (MLR)** model using **SPSS** to predict and optimize the heating loads (Y1) of residential buildings based on their geometric and structural features. 

The dataset comprises 764 distinct building configurations, analyzing how architectural parameters affect energy consumption.

## 🚀 Methodological Rigor & Conclusions
* **High Predictive Power:** Achieved an R^2 score of **0.917**, meaning the model explains **91.7%** of the variance in building heating loads.
* **Multicollinearity Solved:** Identified and resolved severe multicollinearity (VIF > 200) and matrix singularity [X2 = X3 + 2.(X4)] by strategic feature elimination. Final model VIF values are perfectly safe (<10).
* **Autocorrelation Fixed:** Addressed a critical positive autocorrelation issue (DW = 0.580) by implementing **Data Shuffling** to break sequential simulation bias, achieving a near-perfect Durbin-Watson score of **1.991**.
* **Outlier Cleansing:** Detected and removed extreme outliers ($\pm 3\sigma$) using Casewise Diagnostics to ensure katsayı reliability.

---

## 📐 Final Regression Equation

Y1 = -10.160 - 16.511(X1) + 0.032(X3) + 5.754(X5) + 19.747(X7)

### Feature Dictionary:
* **Y1:** Heating Load (Dependent Variable)
* **X1:** Relative Compactness
* **X3:** Wall Area
* **X5:** Overall Height
* **X7:** Glazing Area

---

## 📊 Key Insights
1. **Glazing Area (X7):** Has the strongest positive impact (B = 19.747). Increasing window-to-wall ratios drastically increases the heating load.
2. **Relative Compactness (X1):** Has a powerful negative impact (-16.511). More compact architectural designs reduce heat loss and maximize energy efficiency.
3. **Overall Height (X5):** Taller buildings significantly increase the required heating load (B = 5.754).

---

## 🛠️ Tech Stack & Tools
* **IBM SPSS Statistics** (Regression Analysis, Data Shuffling, Diagnostics)
* **Statistical Methods:** Multicollinearity (VIF & Eigenvalues), Durbin-Watson Autocorrelation Test, Cook's Distance, Casewise Outlier Analysis.
