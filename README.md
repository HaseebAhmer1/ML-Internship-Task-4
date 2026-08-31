# 📊 Task 04 — Statistical Analysis and Hypothesis Testing

## 🎯 Objective

The objective of this task is to apply statistical analysis and hypothesis testing techniques to a real-world health insurance dataset. The analysis focuses on determining whether factors such as smoking status, BMI, age, gender, number of children, and region have statistically significant relationships with medical insurance charges.

The task demonstrates how statistical methods can support evidence-based business decisions, particularly for setting fair and risk-aware insurance premiums.

---

## 📂 Dataset Information

**Dataset Name:** Medical Cost Personal Dataset

**Source:** Kaggle — Medical Cost Personal Dataset

**File:** `insurance.csv`

The dataset contains information about individuals and their medical insurance costs.

### Dataset Features

| Feature | Description | Type |
|---|---|---|
| `age` | Age of the individual | Numerical |
| `sex` | Gender of the individual | Categorical |
| `bmi` | Body Mass Index | Numerical |
| `children` | Number of dependents/children | Numerical |
| `smoker` | Smoking status | Categorical |
| `region` | Residential region | Categorical |
| `charges` | Medical insurance charges | Numerical |

The primary outcome variable used in the analysis is **`charges`**, representing the individual's medical insurance cost.

---

## 🧪 Tasks & Outcomes

### 1. Data Loading and Preprocessing
- Loaded the `insurance.csv` dataset using Pandas.
- Inspected dataset dimensions, columns, data types, and statistical summaries.
- Checked for missing values and duplicate records.
- Identified numerical and categorical variables.
- Documented preprocessing decisions to maintain reproducibility.

### 2. Exploratory Statistical Analysis
- Examined the distribution of medical insurance charges.
- Calculated descriptive statistics such as mean, median, standard deviation, minimum, and maximum.
- Compared insurance charges across different demographic and behavioral groups.
- Used visualizations such as histograms and boxplots to understand data distributions.

### 3. Hypothesis Testing
Applied multiple statistical tests according to the characteristics of the variables:

- **Independent Samples t-test** — compared average insurance charges between smokers and non-smokers.
- **Mann-Whitney U test** — compared the distributions of charges between two independent groups without relying heavily on normality assumptions.
- **Chi-square test** — examined associations between categorical variables such as gender and smoking status.
- **One-way ANOVA** — evaluated whether average insurance charges differed across multiple regions.

### 4. Confidence Intervals
- Calculated confidence intervals for differences in group means.
- Used 95% confidence intervals to quantify the uncertainty around statistical estimates.
- Interpreted whether estimated differences were practically meaningful.

### 5. P-value Interpretation
- Used a significance level of **α = 0.05**.
- Compared calculated p-values against the significance threshold.
- Determined whether sufficient evidence existed to reject the null hypotheses.
- Distinguished statistical significance from practical/business significance.

### 6. Effect Size Analysis
- Calculated **Cohen's d** for comparing two independent groups.
- Used effect sizes to determine the magnitude of observed differences rather than relying only on p-values.

### 7. Multiple Comparison Correction
- Performed pairwise comparisons between regional groups.
- Applied **Bonferroni correction** to control the probability of false-positive findings.
- Compared raw and corrected p-values.

### 8. Statistical Test Selection
Developed reusable helper functions to select appropriate statistical tests based on:

- Number of groups
- Variable type
- Distribution/normality considerations

### 9. Business Interpretation
Translated statistical results into practical insurance-related conclusions, helping evaluate questions such as:

- Do smokers have higher insurance costs?
- Does region significantly affect insurance charges?
- Are categorical characteristics associated with smoking?
- How large are the observed differences?
- Which findings are statistically and practically meaningful?

---

## 🛠️ Key Skills Demonstrated

- Python for statistical analysis
- Pandas for data manipulation
- NumPy for numerical computation
- SciPy for hypothesis testing
- Statsmodels for statistical procedures
- Matplotlib for visualization
- Seaborn for statistical visualization
- Descriptive statistics
- Hypothesis formulation
- Null and alternative hypotheses
- Independent samples t-test
- Welch's t-test
- Mann-Whitney U test
- Chi-square test
- One-way ANOVA
- Confidence interval estimation
- P-value interpretation
- Effect size calculation
- Cohen's d
- Multiple comparison correction
- Bonferroni correction
- Modular and reusable Python functions
- Statistical decision-making
- Business-oriented interpretation

---

## 📚 Key Learnings

### 1. Statistical Testing

Learned how to select and apply statistical tests based on the type of variables, number of groups, and assumptions of the data.

### 2. P-values and Statistical Significance

Learned that a p-value measures the strength of evidence against the null hypothesis. A p-value below the selected significance level provides evidence to reject the null hypothesis.

### 3. Confidence Intervals

Learned how confidence intervals provide a range of plausible values for population parameters and help communicate uncertainty in statistical estimates.

### 4. Effect Sizes

Learned that statistical significance alone is not enough. Effect sizes such as Cohen's d help determine whether a difference is small, moderate, or large in practical terms.

### 5. Parametric vs Non-parametric Tests

Understood when to use parametric tests such as the t-test and ANOVA and when non-parametric alternatives such as Mann-Whitney U may be more appropriate.

### 6. Multiple Comparisons

Learned that performing many statistical tests increases the chance of false-positive results. Multiple comparison corrections such as Bonferroni help control this problem.

### 7. Statistical Assumptions

Learned the importance of checking data distributions and assumptions before selecting a statistical method.

### 8. Business Interpretation

Learned how to translate statistical findings into business insights rather than reporting only test statistics and p-values.

---

## 💼 Business Impact

The analysis provides statistical evidence that can help a health insurance company understand factors associated with medical costs.

Rather than making premium decisions based only on assumptions, the company can use statistical evidence to evaluate differences between customer groups while considering uncertainty, effect magnitude, and the risk of false discoveries.

---

## ✅ Final Outcome

By completing this task, the project demonstrates a complete statistical analysis workflow:

**Data → Cleaning → Exploration → Hypothesis Formation → Test Selection → Statistical Testing → Confidence Intervals → Effect Sizes → Multiple Comparison Correction → Business Interpretation**

The resulting analysis provides a reproducible framework for applying statistical methods to real-world insurance data and communicating findings clearly to both technical and non-technical stakeholders.
