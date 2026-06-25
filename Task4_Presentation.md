# Task 4 Presentation

## Slide 1: Title
- Title: Data Storytelling & Statistical Validation
- Subtitle: E-Commerce Sales Analysis
- Author: Data Analyst Internship Project
- Date: 2026

## Slide 2: Business Problem
- Understand which categories and regions drive revenue.
- Assess whether customer demographics influence order value.
- Provide insights for strategic sales and marketing decisions.

## Slide 3: Dataset Overview
- 1000 cleaned order records.
- 12 columns covering orders, customers, product categories, and revenue.
- Source: `cleaned_dataset.csv`.

## Slide 4: Data Cleaning
- Removed duplicates.
- Imputed numeric missing values with column means.
- Filled missing categorical values as `Unknown`.
- Standardized text values for consistency.

## Slide 5: Exploratory Data Analysis
- Top categories: Electronics, Education, Furniture, Fashion, Grocery.
- Highest total revenue: Electronics.
- Highest average order value: Grocery.
- Leading cities by revenue: Patna, Kolkata, Bengaluru.

## Slide 6: Dashboard Insights
- Power BI visualizes category and city performance.
- Revenue distribution charts confirm the top segments.
- Dashboard supports quick decision-making for sales and regional focus.

## Slide 7: Statistical Validation
- Hypothesis: average order sales differ by gender.
- Test used: Welch's two-sample t-test.
- Result: p-value = 0.495, no significant gender difference.
- Business meaning: gender is not a strong predictor of average order value.

## Slide 8: Business Recommendations
- Invest in Electronics and Grocery growth strategies.
- Optimize regional campaigns for Patna, Kolkata, and Bengaluru.
- Review pricing or bundling for Fashion and Furniture.
- Use gender-neutral promotions for average order value.

## Slide 9: Conclusion
- The dataset is reliable and clean.
- Category and city insights are the strongest levers for revenue.
- Statistical validation supports a focused, data-driven strategy.
- Next step: implement insights in marketing and monitor using Power BI.