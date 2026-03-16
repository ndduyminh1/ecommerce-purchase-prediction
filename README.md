# Predicting Online Shopper Purchase Behavior

<!-- Replace with a short description of the project -->

## Project Overview

An e-commerce company wants to understand which website visitors are most likely to complete a purchase. Only about 15% of visitors currently convert, meaning most traffic does not generate revenue.

The goal of this project is to build a predictive model that identifies high-intent visitors so the company can focus marketing efforts and improve conversion rates.

---

## Business Problem

Online retailers often face low conversion rates despite high website traffic. If the company can identify which visitors are most likely to purchase during their session, they can trigger targeted promotions, personalized recommendations, or incentives to increase revenue.

This project explores behavioral patterns in website sessions and builds a machine learning model to predict purchase outcomes.

---

## Dataset

Dataset: **Online Shoppers Purchasing Intention Dataset**

Source: UCI Machine Learning Repository

Records: **12,330 website sessions**

Target variable:

- **Revenue = True** → visitor completed a purchase  
- **Revenue = False** → visitor did not purchase

Key features include:

- Page visits and browsing behavior
- Session duration
- Bounce and exit rates
- Visitor type (new vs returning)
- Timing information (month, weekend)

---

## Analysis Process

### 1. The Situation

The dataset contains over twelve thousand website sessions with behavioral metrics describing user interactions with an online store. Initial inspection showed no major data quality issues.

Approximately **15% of sessions result in a purchase**, indicating a highly imbalanced classification problem.

---

### 2. The Discovery

Exploratory analysis revealed several behavioral patterns associated with purchasing sessions:

- Returning visitors convert at a higher rate than new visitors.
- Sessions that include more **product-related page visits** are more likely to result in purchases.
- **PageValues** is one of the strongest indicators of purchase intent.

These insights suggest that **user engagement and browsing depth** are key predictors of conversion.

---

### 3. The Model

A **Gaussian Naive Bayes classifier** was trained to predict whether a session would result in a purchase.

Workflow:

- Selected features based on behavioral engagement metrics
- Converted categorical variables using one-hot encoding
- Split data into training and testing sets (80/20 split)
- Evaluated model performance using accuracy and a confusion matrix

The model demonstrates that browsing behavior provides meaningful signals for predicting purchase outcomes.

---

### 4. The Recommendation

Based on the analysis and predictive modeling, the company should consider the following actions:

**1. Trigger promotions for high-engagement visitors**

Visitors who browse multiple product pages and generate higher page values show strong purchase intent. Real-time promotional triggers could increase conversion among these users.

**2. Prioritize returning visitors**

Returning visitors demonstrate higher conversion rates. Personalized recommendations and remarketing campaigns should target these users.

**3. Optimize pages with high exit rates**

High bounce and exit rates correlate with lower conversions. Improving product page clarity, load speed, and checkout flow could reduce abandonment.

**4. Deploy predictive targeting**

The model can be used to identify high-probability buyers in real time, allowing marketing resources to focus on visitors most likely to convert.

---

## Tools Used

Python | Pandas | Scikit-Learn | Matplotlib | Seaborn | Gaussian Naive Bayes | Google Colab

---

*This project was completed as part of ISOM 835: Predictive Analytics at Suffolk University\'s
Sawyer Business School.*
'''

print(readme_template)
