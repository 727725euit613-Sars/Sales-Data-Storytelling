# E-Commerce Sales Storytelling & Statistical Validation

## Project Overview
This project reviews an e-commerce sales dataset to build a business story from data cleaning through exploratory analysis and statistical validation. The analysis focuses on category performance, city revenue, product mix, customer demographics, and decision-ready recommendations.

## Business Problem
The business needs to understand which product categories, cities, and customer segments are driving the highest revenue, and whether demographic groups differ meaningfully in average order value.

## Objective
- Validate the cleaned dataset and ensure reliability.
- Summarize the data cleaning and EDA steps already completed.
- Extract actionable insights from sales, category, city, and gender patterns.
- Perform statistical validation to support decisions with evidence.
- Tell the business story clearly for stakeholders.

## Dataset Description
- Source file: `Data_Wrangling/Task1_Data_Wrangling/cleaned_dataset.csv`
- Records: 1000 orders
- Columns: 12
- Key fields: `Order_ID`, `Order_Date`, `Customer_ID`, `Age`, `Gender`, `City`, `Product`, `Category`, `Quantity`, `Unit_Price`, `Total_Sales`

## Data Cleaning Summary
- Duplicates were identified and removed.
- Numeric missing values were filled using mean imputation.
- Categorical missing values were marked as `Unknown`.
- Text fields were standardized to title case and trimmed.
- The cleaned dataset is stored in `cleaned_dataset.csv` and `cleaned_dataset.xlsx`.

## EDA Summary
- The dataset contains five product categories: `Electronics`, `Education`, `Furniture`, `Fashion`, and `Grocery`.
- `Electronics` is the largest revenue contributor by total sales.
- `Grocery` leads in average sales per order.
- `Patna`, `Kolkata`, and `Bengaluru` generate the most total revenue.
- `Bengaluru` has the highest average order value among cities.
- There is a strong positive correlation between `Unit_Price` and `Total_Sales` and a moderate positive relationship between `Quantity` and `Total_Sales`.

## Dashboard Summary
- The Power BI dashboard summarizes revenue performance by category, city, and customer segment.
- Visualizations include bar charts for category and city revenue, demographic breakdowns, and product-level comparisons.
- The dashboard is available in `Task _ 3.pbix`.

## Key Insights
- `Electronics` is the highest revenue category, accounting for the largest share of sales value.
- `Grocery` has the highest average total sales per order, suggesting strong per-order value in that category.
- `Patna` generates the highest total revenue, while `Bengaluru` shows the highest average order value.
- Gender does not show a statistically significant difference in average `Total_Sales`.
- The strongest numeric drivers of revenue are `Unit_Price` and `Quantity`.

## Business Recommendations
- Prioritize growth investment in `Electronics` and `Grocery` product lines.
- Strengthen regional campaigns for `Patna`, `Kolkata`, and `Bengaluru`.
- Use pricing and product bundling to drive higher per-order value in cities with lower average sales.
- Maintain a gender-neutral approach for average order value marketing, and focus segmentation by geography and category instead.
- Review performance improvement opportunities in `Fashion` and `Furniture` given their lower average order values.

## Technologies Used
- Python
- pandas
- numpy
- scipy
- matplotlib
- seaborn
- Power BI

## Folder Structure
- `Data_Wrangling/Task1_Data_Wrangling/` — raw and cleaned dataset, cleaning script, data dictionary
- `EDA-Business-Intelligence/EDA_Project/` — EDA report, analysis script, dashboard resources, SQL queries
- `Task _ 3.pbix` — Power BI dashboard file
- `README.md` — project-level overview and summary
- `Business_Story.md` — business storytelling narrative
- `Hypothesis_Testing.md` — hypothesis test documentation
- `Task4_Data_Storytelling.ipynb` — executable Task 4 notebook
- `Task4_Presentation.md` — presentation slide content
- `requirements.txt` — Python package requirements

## Conclusion
The project is ready for stakeholder review with a clean dataset, clear analytics narrative, and evidence-backed statistical validation. Removing unnecessary folders such as `venv`, `.venv`, `__pycache__`, and `node_modules` will make the repository presentation-ready for internship or professional submission.# Sales-Data-Storytelling
