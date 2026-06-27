# Regression Model Equations & Interpretation

## 1. Simple Regression Equations
Based on the isolated regression outputs, the equations for our single-variable models are:
* **Model 1 (Marketing Spend):** $Monthly sales = 618583.57 + 0.28(Marketing Spend)$
  * *Interpretation:* When isolated, marketing spend shows a massive baseline intercept but only generates $0.28 for every dollar spent. It is statistically significant (P-value: 0.001) but practically inefficient.
* **Model 2 (Footfall):** $Monthly\_Sales = 17947.29 + 75.98(Footfall)$
  * *Interpretation:* When isolated, footfall is a highly significant driver (P-value: 1.15E-11), generating $75.98 in top-line sales per visitor.

## 2. Multiple Regression Equation (Final Model)
Based on the comprehensive multiple regression analysis, the predictive equation for monthly store sales is:

$Monthly\_Sales = -47395.73 + 0.29(Marketing\_Spend) + 63.63(Footfall) + 1481.54(Inventory\_Pct) + 3147.26(is\_Mall) + 39912.44(is\_High\_Street) + 115216.51(is\_Airport)$

## 3. Coefficient Explanations & Business Impact (Final Model)
* **Intercept (-47,395.73):** The theoretical baseline sales if all other variables were zero. In business terms, this represents fixed overhead drag; a store with zero traffic, zero inventory, and zero marketing operates at a loss.
* **marketing_spend (0.29):** For every $1.00 spent on marketing, monthly sales increase by only $0.29. **This is a negative ROI.** Marketing is currently burning cash.
* **footfall (63.63):** Every additional visitor entering the store equates to $63.63 in top-line sales.
* **inventory_availability_pct (1481.54):** For every 1% improvement in inventory availability, sales increase by $1,481.54. Keeping shelves stocked is highly lucrative.

## 4. Dummy Variable Explanation
Categorical variables (`store_type`) cannot be read by regression algorithms. We transformed the 4 store types into binary variables (1 or 0). 
* **Reference Category Used:** **Residential**. We omitted the "Residential" dummy to serve as our mathematical baseline.
* **Interpretation:** The coefficients for the included dummies represent their performance *compared to Residential stores*. For example, the `is_Airport` coefficient is 115,216.51. This means holding all other variables (traffic, inventory, marketing) equal, an Airport store will generate $115,216.51 more in monthly sales than a Residential store.

## 5. Final Model Selection
The Multiple Regression model is selected as the definitive operational model. It yields an R-squared of ~0.82 (explaining 82% of sales variance), vastly outperforming the isolated marketing (0.08) and footfall (0.38) models. All included variables possess P-values well below the 0.05 threshold, proving strong statistical significance across the board.
