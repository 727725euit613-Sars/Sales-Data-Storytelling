# Hypothesis Testing

## Business Question
Does average order `Total_Sales` differ between male and female customers?

## Null Hypothesis (H0)
The average `Total_Sales` for male customers is equal to the average `Total_Sales` for female customers.

## Alternative Hypothesis (H1)
The average `Total_Sales` for male customers is not equal to the average `Total_Sales` for female customers.

## Statistical Test Used
- Independent two-sample t-test (Welch's t-test)

## Why this test was selected
- The target variable (`Total_Sales`) is continuous.
- There are two independent groups defined by `Gender`.
- The test does not require equal population variances.

## Python Code
```python
import pandas as pd
from scipy.stats import ttest_ind, levene

# Load cleaned dataset
path = 'Data_Wrangling/Task1_Data_Wrangling/cleaned_dataset.csv'
df = pd.read_csv(path)

define_date = pd.to_datetime(df['Order_Date'], errors='coerce')

male_sales = df[df['Gender'] == 'Male']['Total_Sales']
female_sales = df[df['Gender'] == 'Female']['Total_Sales']

# Variance homogeneity check
levene_result = levene(male_sales, female_sales)
print('Levene p-value:', levene_result.pvalue)

# Welch's t-test for unequal variances
ttest_result = ttest_ind(male_sales, female_sales, equal_var=False)
print('t-statistic:', ttest_result.statistic)
print('p-value:', ttest_result.pvalue)
```

## p-value Interpretation
- Observed p-value: `0.4950`.
- Because the p-value is greater than the common 0.05 threshold, we fail to reject the null hypothesis.
- There is no statistically significant evidence that average `Total_Sales` differs by gender.

## Business Conclusion
The data shows that male and female customers have comparable average order values. This suggests the business should focus segmentation and promotional investment on product categories and high-performing cities rather than gender for average order value optimization.