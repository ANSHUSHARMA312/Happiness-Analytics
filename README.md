# Understanding the Drivers of National Well-Being

A data-driven exploration of global happiness using dimensionality reduction, clustering, predictive modeling, and a custom Happiness Efficiency Index (HEI).

---

## Overview

What makes nations happy?

This project investigates the socioeconomic determinants of happiness across **157 countries** using data from the **World Happiness Report**. The analysis combines statistical modeling and machine learning techniques to identify key drivers of well-being, uncover country archetypes, and quantify countries that perform better or worse than expected.

---

## Objectives

* Analyze the relationship between happiness and socioeconomic indicators.
* Identify the strongest predictors of happiness.
* Reduce dimensionality using Principal Component Analysis (PCA).
* Segment countries into meaningful groups using clustering.
* Predict happiness scores using regression models.
* Develop a Happiness Efficiency Index (HEI) to identify overperforming and underperforming nations.

---

## Dataset

**Source:** World Happiness Report

**Observations:** 157 Countries

### Features Used

* Economy (GDP per Capita)
* Family (Social Support)
* Health (Life Expectancy)
* Freedom
* Trust (Government Corruption)
* Generosity
* Happiness Score

---

## Methodology

### 1. Exploratory Data Analysis (EDA)

* Top 10 Happiest Countries
* GDP vs Happiness Relationship
* Correlation Analysis
* Correlation Heatmap

### 2. Principal Component Analysis (PCA)

Reduced six correlated socioeconomic indicators into four principal components while retaining:

**91.7% of total variance**

Key latent dimensions identified:

* Socioeconomic Development
* Social Capital & Institutional Trust

### 3. Country Segmentation

Applied **K-Means Clustering** to identify four well-being archetypes:

* High-Performing Developed Nations
* Emerging Prosperous Nations
* Institutionally Weak Economies
* Vulnerable Economies

### 4. Happiness Prediction

Built a Linear Regression model to predict national happiness scores.

**Performance**

| Metric   | Value |
| -------- | ----- |
| R² Score | 0.71  |
| MAE      | 0.50  |

### 5. Happiness Efficiency Index (HEI)

Custom metric:

HEI = Actual Happiness − Predicted Happiness

The index highlights countries that are significantly happier or less happy than expected given their socioeconomic indicators.

---

## Key Findings

### Health Matters Most

Regression coefficients showed:

1. Health (Life Expectancy)
2. Freedom
3. Family (Social Support)
4. GDP
5. Trust
6. Generosity

Health emerged as the strongest predictor of happiness.

---

### Wealth Alone Is Not Enough

Although GDP exhibited a strong correlation with happiness, regression analysis revealed that freedom and social support contribute more strongly after controlling for other factors.

---

### Four Distinct Well-Being Archetypes Exist

Countries naturally cluster into distinct socioeconomic and happiness profiles, demonstrating that well-being is multidimensional.

---

### Happiness Overperformers

Countries such as:

* Costa Rica
* Mexico
* Brazil
* Pakistan
* Israel

reported happiness levels significantly above model expectations.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

## Repository Structure

```text
Happiness-Analytics/
│
├── data/
├── notebooks/
│   └── Happiness_Analysis.ipynb
│
├── images/
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

## Future Improvements

* XGBoost-based prediction models
* SHAP explainability analysis
* Interactive dashboard using Streamlit
* Multi-year World Happiness Report analysis

---

## Author

**Anshu Sharma**

Chemical Engineering, IIT Kanpur
