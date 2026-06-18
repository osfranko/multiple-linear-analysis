# 📊 Multiple Linear Regression – Multi-Channel Marketing Analysis

## 🎯 Project Overview
This project applies **Multiple Linear Regression (MLR)** to analyze the relationship between marketing spend and sales performance across multiple advertising channels.

The objective is to determine which marketing channels (TV, Radio, Social Media, and Influencer type) significantly influence **Sales**, and to use statistical evidence to guide business decision-making.

---

## 📌 Project Goal
By the end of this analysis, the project achieves the following:

- Detect multicollinearity among predictors
- Build a statistically valid Multiple Linear Regression model
- Evaluate model performance using Adjusted R² and p-values
- Validate regression assumptions using diagnostic plots
- Interpret coefficients in a business context
- Provide data-driven marketing recommendations

---

## 📂 Dataset Description
The dataset contains **200 observations** with the following variables:

- **TV**: Advertising spend on TV
- **Radio**: Advertising spend on Radio
- **Social Media**: Advertising spend on Social Media
- **Influencer**: Influencer category (Micro, Macro, Mega, Nano)
- **Sales**: Target variable (sales generated)

---

## 🧰 Technologies Used
- Python 🐍
- Pandas
- NumPy
- Seaborn & Matplotlib
- Statsmodels (OLS Regression)
- SciPy

---

## 📌 Step-by-Step Project Tasks

### 1. Load Dataset & Exploratory Data Analysis (EDA)
- Imported dataset using Pandas
- Checked dataset shape, data types, and missing values
- Generated descriptive statistics
- Visualized Sales distribution

---

### 2. Multicollinearity Check
Checked relationships among independent variables (TV, Radio, Social Media) using:

- Correlation matrix (heatmap visualization)
- Variance Inflation Factor (VIF)

📌 **Result:**
- All VIF values < 5
- No severe multicollinearity detected

---

### 3. Multiple Linear Regression Model
Built a regression model using **Statsmodels OLS**:

- Converted categorical variable (Influencer) using one-hot encoding
- Ensured all variables were numeric
- Added constant term
- Fitted OLS regression model

---

### 4. Model Performance Evaluation
Model evaluated using:

- Adjusted R-squared
- Individual predictor p-values
- F-statistic significance

📌 **Key Results:**
- Adjusted R² ≈ 0.102
- Model is statistically significant overall
- TV and Radio are significant predictors

---

### 5. Diagnostic Checks (Model Assumptions)
Regression assumptions were validated using:

- Residuals vs Fitted plot → Linearity & Homoscedasticity
- Q-Q Plot → Normality of residuals
- Histogram of residuals → Distribution check

📌 **Conclusion:**
- Residuals are randomly distributed
- No major violations of assumptions
- Model is valid for inference

---

### 6. Coefficient Interpretation (Business Context)

Interpretation assumes **holding all other variables constant**:

- 📺 **TV (0.0354)**: Each $1 increase in TV spend increases Sales by ~0.035 units
- 📻 **Radio (0.2262)**: Each $1 increase in Radio spend increases Sales by ~0.226 units (strongest effect)
- 📱 **Social Media (0.0090)**: Weak and not statistically significant
- 🎯 **Influencer Types**: Not statistically significant overall

---

### 7. Business Recommendation

Based on model results:

#### 📌 Key Insights
- Radio advertising has the highest impact on sales
- TV advertising is the second strongest driver
- Social Media shows weak predictive power
- Influencer marketing is not statistically reliable in this dataset

#### 📊 Final Recommendation
- Increase investment in **Radio advertising**
- Maintain or moderately increase **TV advertising**
- Re-evaluate or optimize **Social Media strategy**
- Test and refine **Influencer marketing campaigns**

---

## 📊 Final Model Summary
- Adjusted R²: ~0.102
- Significant predictors: TV, Radio
- Model is statistically valid for interpretation
- Assumptions are reasonably satisfied

## 📁 Project Submission Checklist

This GitHub repository includes:

✔ Jupyter Notebook (`multiple_regression_analysis.ipynb`)  
✔ Full regression analysis with outputs  
✔ Data preprocessing and encoding steps  
✔ Diagnostic plots and interpretation  
✔ Clean Markdown explanations  

## ⚙️ Installation Requirements

To run this project:

```bash
pip install pandas numpy matplotlib seaborn statsmodels scipy
Author: Osemwengie Osasere 
