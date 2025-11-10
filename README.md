# 📊 Telco Customer Churn Analysis

A comprehensive data analysis project to understand customer churn patterns in a telecommunications company. This analysis explores various factors affecting customer retention and identifies key indicators of customer churn.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Key Findings](#key-findings)
- [Installation & Setup](#installation--setup)
- [Analysis Process](#analysis-process)
- [Visualizations](#visualizations)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Author](#author)

---

## 🎯 Project Overview

This project analyzes customer churn data from a telecommunications company to identify patterns and factors that contribute to customer attrition. The analysis helps understand:

- Customer demographics and their impact on churn
- Service usage patterns
- Contract types and payment methods
- Key factors driving customer retention

**Key Metrics:**
- 📊 Total Customers: 7,043
- 🚫 Churned Customers: 1,869 (26.54%)
- ✅ Retained Customers: 5,174 (73.46%)

---

## 📚 Dataset Description

**Dataset:** Telco-Customer-Churn.csv

**Size:** 7,043 rows × 21 columns

### Column Descriptions

| Column | Description | Type |
|--------|-------------|------|
| `customerID` | Unique customer identifier | Object |
| `gender` | Customer gender (Male/Female) | Object |
| `SeniorCitizen` | Whether customer is senior citizen (Yes/No) | Object |
| `Partner` | Whether customer has partner (Yes/No) | Object |
| `Dependents` | Whether customer has dependents (Yes/No) | Object |
| `tenure` | Number of months customer stayed | Integer |
| `PhoneService` | Whether customer has phone service | Object |
| `MultipleLines` | Whether customer has multiple lines | Object |
| `InternetService` | Type of internet service (DSL/Fiber optic/No) | Object |
| `OnlineSecurity` | Whether customer has online security | Object |
| `OnlineBackup` | Whether customer has online backup | Object |
| `DeviceProtection` | Whether customer has device protection | Object |
| `TechSupport` | Whether customer has tech support | Object |
| `StreamingTV` | Whether customer has streaming TV | Object |
| `StreamingMovies` | Whether customer has streaming movies | Object |
| `Contract` | Contract type (Month-to-month/One year/Two year) | Object |
| `PaperlessBilling` | Whether customer uses paperless billing | Object |
| `PaymentMethod` | Payment method used | Object |
| `MonthlyCharges` | Monthly charges amount | Float |
| `TotalCharges` | Total charges amount | Float |
| `Churn` | Whether customer churned (Yes/No) | Object |

---

## 🔍 Key Findings

### 1️⃣ Overall Churn Rate
- **26.54%** of customers have churned
- **73.46%** of customers are retained
- Churn is a significant concern requiring immediate attention

### 2️⃣ Senior Citizens
- **Comparatively greater percentage** of senior citizens have churned
- Senior citizens show higher churn rates than non-senior citizens
- Special retention strategies needed for this demographic

### 3️⃣ Tenure Analysis
- Customers with **longer tenure (high months)** tend to stay
- Customers who used services for **1-2 months** are more likely to churn
- First few months are critical for customer retention

### 4️⃣ Contract Type Impact
- **Month-to-month contracts** have the highest churn rate
- Customers with **1-year or 2-year contracts** are more likely to stay
- Long-term contracts significantly improve retention

### 5️⃣ Payment Method
- Customers using **Electronic check** payment method show higher churn
- Other payment methods (Bank transfer, Credit card, Mailed check) have better retention

### 6️⃣ Gender Analysis
- Gender does **not significantly impact** churn rates
- Both male and female customers churn at similar rates

---

## 🛠️ Installation & Setup

### Prerequisites

- Python 3.7 or higher
- Jupyter Notebook or JupyterLab

### Required Libraries

```bash
pip install pandas numpy matplotlib seaborn
```

---

## 📁 Analysis Process

### Step 1: Data Loading & Exploration
- Loaded Telco-Customer-Churn.csv dataset
- Explored data structure with 7,043 rows and 21 columns
- Checked data types and statistical summary

### Step 2: Data Cleaning
1. ✅ **Handled Missing Values:**
   - Identified blank values in `TotalCharges` column
   - Replaced blank spaces with 0 (customers with 0 tenure)
   - Converted `TotalCharges` from object to float

2. ✅ **Checked for Duplicates:**
   - No duplicate records found
   - No duplicate customer IDs

3. ✅ **Data Transformation:**
   - Converted `SeniorCitizen` from binary (0/1) to categorical (yes/no)
   - Improved data readability

### Step 3: Exploratory Data Analysis (EDA)
- Analyzed churn distribution
- Examined categorical variables impact on churn
- Studied numerical features (tenure, charges)
- Created multiple visualizations

### Step 4: Data Visualization
Created comprehensive visualizations including:
- Count plots for churn distribution
- Pie chart for churn percentage
- Gender-wise churn analysis
- Senior citizen churn patterns
- Tenure distribution by churn
- Contract type impact
- Payment method analysis
- Multi-panel categorical analysis

---

## 📊 Visualizations

### 1. Churn Distribution
- Count plot showing churned vs retained customers
- Pie chart displaying 26.54% churn rate

### 2. Gender Analysis
- Countplot comparing male vs female churn rates
- Minimal difference observed

### 3. Senior Citizen Impact
- Stacked bar chart with percentages
- Shows higher churn rate among senior citizens

### 4. Tenure Analysis
- Histogram with bins showing tenure distribution
- Clear pattern: longer tenure = lower churn

### 5. Contract Type
- Countplot showing month-to-month contracts have highest churn
- Long-term contracts significantly reduce churn

### 6. Payment Method
- Electronic check users show highest churn
- Other payment methods perform better

### 7. Multi-Variable Analysis
- Grid of countplots for all categorical variables
- Comprehensive view of factors affecting churn

---

## 💻 Technologies Used

- **Python 3** - Programming Language
- **Pandas** - Data Manipulation and Analysis
- **NumPy** - Numerical Computing
- **Matplotlib** - Data Visualization
- **Seaborn** - Statistical Data Visualization
- **Jupyter Notebook** - Interactive Development Environment

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/telco-churn-analysis.git
   cd telco-churn-analysis
   ```

2. **Install required libraries:**
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

3. **Ensure dataset is available:**
   - Place `Telco-Customer-Churn.csv` in the project directory

4. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook analysis.ipynb
   ```

5. **Run all cells** to reproduce the analysis

---

## 📈 Business Recommendations

Based on the analysis, here are key recommendations:

1. 🎯 **Focus on Early Engagement**
   - Implement onboarding programs for new customers
   - Provide special offers in first 3 months

2. 📝 **Promote Long-term Contracts**
   - Incentivize 1-year and 2-year contracts
   - Offer discounts for contract upgrades

3. 👴 **Senior Citizen Retention Program**
   - Create targeted retention strategies
   - Provide personalized support

4. 💳 **Optimize Payment Methods**
   - Encourage customers to switch from Electronic check
   - Promote automatic payment methods

5. 📞 **Improve Customer Support**
   - Enhanced tech support for at-risk customers
   - Proactive outreach to month-to-month contract holders

---

## 🔮 Future Enhancements

- [ ] Build predictive machine learning model to predict churn
- [ ] Create interactive dashboard using Plotly or Streamlit
- [ ] Perform customer segmentation analysis
- [ ] Add time-series analysis for churn trends
- [ ] Implement feature importance analysis

---

## 📞 Contact

For questions, feedback, or collaboration:
- 🔗 LinkedIn: [linkedin.com/in/sonu-kumar-65ab85255](https://www.linkedin.com/in/sonu-kumar-65ab85255)
- 🌐 GitHub: [github.com/Sonujack](https://github.com/Sonujack)

---

## 📄 License

This project is open source and available under the MIT License.

---

