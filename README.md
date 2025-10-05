# 🧬 VitalMetrics – Life Expectancy Prediction Model  

VitalMetrics is a statistical modeling project that explores how socioeconomic and health factors influence global life expectancy.  
Using real-world WHO data across 193 countries, the project applies rigorous data cleaning, feature selection, and regression analysis to uncover patterns that drive longevity.

---

## 🌍 Overview  

This project investigates the relationship between **life expectancy** and key predictors such as:  
- Income Composition of Resources  
- Schooling (Years of Education)  
- Body Mass Index (BMI)  
- Adult Mortality Rate  
- HIV/AIDS Prevalence  

The goal is to identify which factors most strongly influence life expectancy and to create a reliable model for predicting it across diverse regions.

---

## 📊 Methodology  

1. **Data Source**  
   - WHO Life Expectancy dataset (via Kaggle) containing socioeconomic and health indicators from 193 countries.  

2. **Data Preparation**  
   - Removed missing values and handled outliers.  
   - Verified assumptions of linearity, independence, and homoscedasticity.  
   - Conducted exploratory analysis using scatter plots, QQ plots, and residual diagnostics.  

3. **Model Development**  
   - Built a **Multiple Linear Regression (MLR)** model with AIC/BIC-based variable selection.  
   - Applied **cross-validation** to assess model robustness and predictive reliability.  
   - Final model achieved an **Adjusted R² of 0.878**, indicating strong explanatory power.  

4. **Validation & Interpretation**  
   - Checked multicollinearity using Variance Inflation Factor (VIF).  
   - Performed Box-Cox transformations to normalize skewed distributions.  
   - Interpreted coefficients to quantify the effect of each predictor on life expectancy.

---

## 🧠 Key Insights  

- **Income Composition** had the strongest positive correlation with life expectancy.  
- **Schooling** and **BMI** also showed moderate positive associations.  
- **Adult Mortality** and **HIV/AIDS** were negatively associated, indicating their significant impact on reducing life expectancy.  
- The model’s validation confirmed its accuracy and generalizability across countries.  

---

## ⚙️ Tools & Technologies  

- **R** – Statistical analysis and visualization  
- **ggplot2**, **car**, **MASS** – Regression diagnostics, transformations, and visualization  
- **dplyr** – Data manipulation  
- **tidyr** – Data cleaning  

---

## 📈 Example Output  

| Predictor | Coefficient | Interpretation |
|------------|-------------|----------------|
| Income Composition | +22.26 | 1-unit increase raises life expectancy by ~22 years |
| Adult Mortality | -0.02 | 1-unit increase decreases life expectancy by ~0.02 years |
| HIV/AIDS | -0.45 | Higher prevalence reduces overall life expectancy |

---

## 💡 Learnings  

- Reinforced skills in **data modeling**, **feature selection**, and **statistical inference**.  
- Strengthened understanding of how **socioeconomic factors shape health outcomes** globally.  
- Gained hands-on experience validating models for predictive accuracy and interpretability.

---

## 📚 Dataset  

[WHO Life Expectancy Dataset on Kaggle](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who)
