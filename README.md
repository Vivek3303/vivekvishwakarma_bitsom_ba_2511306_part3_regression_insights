# vivekvishwakarma_bitsom_ba_2511306_part3_regression_insights
# Part 3: Regression-Based Business Insights

## Business Problem Summary
The retail leadership team requires a data-driven strategy to maximize monthly sales. By applying regression analysis to operational data, this project identifies the exact monetary impact of marketing, footfall, inventory, and store locations to recommend high-ROI business actions.

## Dataset Description
- **Source:** `business_regression_data.xlsx`
- **Scope:** Store-level performance metrics, including physical location types, monthly overhead, traffic, and revenue.

## Variables Identified
- **Dependent Variable:** `monthly_sales`
- **Independent Variables (Numerical):** `marketing_spend`, `footfall`, `inventory_availability_pct`.
- **Independent Variables (Categorical/Dummy):** `store_type` (Residential, Mall, High Street, Airport).

## Regression Approach & Dummy Variables
Categorical `store_type` data was converted into binary dummy variables. "Residential" was utilized as the baseline reference category to prevent multicollinearity (the dummy variable trap). Multiple regression was executed using Excel's Data Analysis Toolpak to isolate the coefficients and P-values of each independent variable.

## Model Comparison Summary
The final Multiple Regression model (R-squared: 0.8199) vastly outperformed isolated simple regressions. It successfully mapped 82% of sales variance to the independent variables, all of which returned statistically significant P-values (< 0.05). 

## Final Business Recommendation
1. **Scale Inventory & Premium Real Estate:** Inventory availability drives high returns (+$1,481 per 1%), and Airport/High Street locations mathematically dominate Residential zones.
2. **Audit Marketing:** Marketing spend currently has a negative ROI (returning only $0.29 per $1.00 spent). Reallocate marketing capital into supply chain and footfall-driving initiatives.

## Assumptions & Limitations
The model assumes linear relationships across all variables and does not factor in external macroeconomic volatility, localized competitor actions, or qualitative operational metrics like employee morale.

## Screenshots Included
- `simple_regression_output.png`
- `multiple_regression_output.png`
- `residuals_preview.png`
- `model_comparison_preview.png`
