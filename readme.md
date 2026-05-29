# 📊 Statistical Data Analysis & Visualization Project

## 📌 Project Overview

This project presents the final report of a Data Analyst sprint focused on mastering fundamental statistical concepts and applying them to real-world datasets.

The project combines:
- Statistical theory
- Exploratory Data Analysis (EDA)
- Hypothesis testing
- Data visualization
- Business & scientific interpretation

Two datasets were analyzed:
1. Public Health Expenditure Dataset
2. Automobile MPG Dataset

---

# 🎯 Objectives

- Understand and apply descriptive statistics
- Explore probability distributions and hypothesis testing
- Perform real-world exploratory data analysis
- Detect trends, correlations, and anomalies
- Build insightful visualizations
- Interpret statistical results for decision-making

---

# 🛠️ Phase 1 — Statistical Foundations

This phase focused on mastering the theoretical foundations required for reliable data analysis.

## 📚 Statistical Concepts Covered

### Descriptive Statistics
- Mean
- Median
- Variance
- Standard deviation
- Histogram
- Boxplot

### Population vs Sample
- Definitions
- Sampling methods
- Sampling bias

### Probability & Distributions
- Bernoulli Distribution
- Binomial Distribution
- Poisson Distribution
- Normal (Gaussian) Distribution
- Student Distribution
- Chi-Square Distribution

### Central Limit Theorem (CLT)
Understanding how sample means approximate a normal distribution.

### Estimation & Confidence Intervals
- Bias evaluation
- Confidence intervals
- Sampling estimation

### Hypothesis Testing
- Null hypothesis (H0)
- Alternative hypothesis (H1)
- p-value interpretation
- Decision making using significance level α

---

# 🏥 Phase 2 — Public Health Data Analysis

## Dataset
`healthexp.csv`

Dataset containing worldwide healthcare expenditure and life expectancy data.

---

# 📈 Key Analyses & Insights

## Nature of Variables

### Continuous Variables
- Spending_USD
- Life_Expectancy

### Categorical / Discrete Variables
- Year
- Country

---

## Spending_USD Analysis

### Univariate Analysis
- Histogram and boxplot revealed strong right-skewness
- US healthcare spending acts as a major outlier

### Mean Interpretation
The mean of `Spending_USD` represents the average healthcare spending per capita across all countries and years.

This average is heavily influenced by extremely high US spending values.

---

## Time Series Analysis

### Life Expectancy Evolution
- General upward trend across most countries
- Noticeable stagnation in recent years in the United States

### Germany vs United Kingdom
Germany consistently spends more on healthcare than the UK while following similar trends.

---

## Correlation & Outliers

### Spending vs Life Expectancy (USA)
A strong positive Pearson correlation (~0.9+) was observed between healthcare spending and life expectancy.

### Statistical Significance
The associated p-value was near zero, indicating the relationship is statistically significant.

### Major Outlier
The United States represents the strongest anomaly:
- Extremely high healthcare spending
- Lower life expectancy than several lower-spending countries

---

## Advanced Statistical Analysis

### Hypothesis Testing
A statistical hypothesis test was performed on the claim:

> “US life expectancy increased by +0.3 years annually since 1970”

Using:
- Confidence level: 98%
- α = 0.02

---

# 🚗 Phase 3 — Automobile MPG Analysis

## Dataset
`MPG Dataset`

Dataset containing fuel consumption and vehicle characteristics from 1970–1982.

---

# 📈 Key Analyses & Insights

## Nature of Variables

### Continuous Variables
- mpg
- horsepower
- weight
- acceleration

### Categorical / Discrete Variables
- cylinders
- model_year
- origin

---

## MPG Analysis

### Mean Interpretation
The mean MPG represents the average fuel efficiency of all vehicles in the dataset.

Higher MPG values indicate lower fuel consumption.

### Distribution Analysis
Histogram and boxplot revealed:
- Wide distribution
- Majority of vehicles between 15–30 MPG
- Presence of highly fuel-efficient vehicles

---

## Key Relationships

### MPG vs Horsepower
Strong negative correlation:
- Higher horsepower → Lower MPG
- More power → More fuel consumption

### Effect of Model Year
Newer vehicles tend to achieve:
- Better MPG
- Improved efficiency for similar horsepower

---

## Vehicle Weight Evolution

US vehicles showed a clear decrease in average weight beginning in the late 1970s.

This reflects industry adaptation to:
- Fuel efficiency concerns
- Economic changes
- Oil crisis impacts

---

## Cylinders vs Model Year

The scatterplot revealed a historical transition:
- Early 1970s dominated by 8-cylinder engines
- Gradual shift toward 4-cylinder engines

This phenomenon reflects:
- Engine downsizing
- Improved fuel economy strategies

---

# 📊 Visualizations Created

| Visualization | Purpose |
|---|---|
| Histogram | Distribution analysis |
| Boxplot | Outlier detection |
| Scatterplot | Correlation analysis |
| Time Series | Trend evolution |
| Comparative Charts | Country & vehicle comparisons |

---

# 🧠 Key Learnings

- Real-world datasets often contain strong outliers
- Correlation does not always imply efficiency
- Statistical tests validate whether relationships are significant
- Visualization is essential for interpreting trends and anomalies
- Fuel efficiency improved significantly after the 1970s

---

# 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Data analysis |
| Pandas | Data manipulation |
| NumPy | Numerical computations |
| Matplotlib | Visualization |
| Seaborn | Statistical graphics |
| SciPy | Statistical testing |
| Jupyter Notebook | Analysis environment |

---

# 📂 Repository Structure

```bash
📦 statistical-analysis-project/
├── data/
│   ├── healthexp.csv
│   ├── mpg.csv
│
├── notebooks/
│   ├── health_analysis.ipynb
│   ├── mpg_analysis.ipynb
│
├── assets/
│   ├── visualizations.png
│
├── README.md
└── requirements.txt
```

---

# 🚀 Possible Extensions

- Add predictive modeling
- Build interactive dashboards
- Integrate machine learning algorithms
- Deploy visualizations with Streamlit

---

# 👨‍💻 Author

**Zoubair Baladi**  
🎓 Master's Degree in Systems & Telecommunications  
📊 Passionate about Data Engineering, Data Analysis & Business Intelligence

🔗 LinkedIn:
https://www.linkedin.com/in/zoubair-baladi/


