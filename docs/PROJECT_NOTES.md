# Project Notes

## Analysis flow

Raw customer data → quality checks → cleaning → feature engineering → exploratory analysis → campaign comparison → customer segmentation → dashboard/reporting.

## Main calculated fields

**Age**  
Calculated from the recorded birth year using the project reference year.

**Total Spending**  
Sum of spending across wine, fruit, meat, fish, sweets, and gold products.

**Total Purchases**  
Sum of web, catalog, and store purchases.

**Total Campaign Accepted**  
Sum of the five campaign acceptance fields.

**Children**  
Combined count of children and teenagers in the household.

**Parental Status**  
Customers with one or more children/teenagers were classified as parents; others were classified as non-parents.

**Customer Tenure**  
Calculated from the customer signup date to the project reference date.

## Data-quality decisions

- Missing income values were filled with the median income.
- Very high income values were flagged so they would not distort the analysis.
- Ages above 100 were treated as invalid for the analysis and set to missing.
- Date fields were converted to proper date types.

## Business interpretation

The strongest pattern in this analysis was the difference between campaign responders and non-responders. Responders showed higher average spending and purchasing activity, suggesting that campaign response can be useful when identifying higher-value customer groups.

The analysis also showed that campaign performance was not equal across all five campaigns. Campaign 4 had the highest number of acceptances.

## Important note

The notebook contains the analysis workflow, while the Power BI file contains the dashboard/reporting work. The database connection code in the public copy has been replaced with a safe placeholder so that credentials are not committed to GitHub.
