# 📧 A/B Test & Predictive Modeling on Email Marketing Campaign

This project explores the effectiveness of offering discounts in email marketing campaigns using both statistical testing and machine learning techniques. The goal is to understand whether offering a discount significantly impacts purchase behavior and to predict which users are most likely to convert.

---

## 🔍 Objective

* **A/B Testing**: Compare purchase rates between two groups—those who received a discount and those who didn’t.
* **Predictive Modeling**: Use logistic regression and a random forest classifier to predict purchase likelihood based on user demographics and behavior.

---

## 📁 Dataset

The dataset includes information for 20 customers and contains the following features:

* `Customer id`
* `Age`
* `Gender` (0 = Male, 1 = Female)
* `Location`
* `Email Opened`
* `Email Clicked`
* `Product Page Visit`
* `Discount Offered` (0 = No, 1 = Yes)
* `Purchased` (Target variable)

---

## 🧪 A/B Testing Process

We divided users into two groups:

* **Group A**: No discount
* **Group B**: Discount offered

We used a **two-proportion z-test** to test the difference in conversion rates between these groups.

> **Result**: The p-value was \~0.073, which is slightly above the typical 0.05 threshold. This means the discount group showed higher purchase rates, but the result wasn't statistically significant at the 95% confidence level.

---

## 🤖 Predictive Modeling

We applied two models:

1. **Logistic Regression**

   * Very low predictive accuracy due to the small dataset.
   * Failed to correctly identify purchasers.

2. **Random Forest Classifier**

   * Improved performance slightly (accuracy \~33%).
   * Top features: Age, Product Page Visit, and Discount Offered.

> Note: The dataset is very small, so the models are not production-ready but demonstrate the pipeline and feature importance logic.

---

## 📊 Visuals & Insights

* **Bar Chart** showing purchase rate by discount
* **Confusion Matrix** to evaluate model performance
* **Feature Importance** chart to highlight key predictors

---

## 📌 Conclusion

* **Discounts may influence purchases**, but more data is needed to confirm statistically.
* **Age and engagement metrics** like page visits are strong predictors of conversions.
* This project lays the foundation for scaling up analysis on larger campaigns with improved accuracy.

---

## 🚀 How to Run

1. Install the required libraries:

   ```bash
   pip install pandas matplotlib seaborn scikit-learn
   ```

2. Open and run the Jupyter Notebook:
   `A:B Test on Email Marketing Campaign.ipynb`

---



