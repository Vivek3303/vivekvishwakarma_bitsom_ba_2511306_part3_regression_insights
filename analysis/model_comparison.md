# Regression Model Comparison

| Required Item | Explanation |
| :--- | :--- |
| **Model Names** | Simple Reg 1 (Marketing), Simple Reg 2 (Footfall), Multiple Reg (Comprehensive). |
| **Variables Used** | **Dependent:** `monthly_sales`. <br>**Independent:** `marketing_spend`, `footfall`, `inventory_availability_pct`, `is_Mall`, `is_High_Street`, `is_Airport`. |
| **R-squared Analysis** | The Multiple Regression model achieved an R-squared of 0.8199. This indicates that roughly 82% of the variance in monthly sales is explained by this specific combination of variables, vastly outperforming any isolated simple regression. |
| **Significant Variables** | Every variable in the final multiple regression model yielded a P-value < 0.05 (ranging from 1.48E-58 to 2.37E-12). All variables are statistically significant. |
| **Business Usefulness** | Highly useful. The model isolates the exact monetary value of inventory (+$1.4k per 1%) and footfall (+$63 per person), while mathematically proving that current marketing spend is inefficient (generating only $0.29 on the dollar). |
| **Limitations** | The model assumes linear relationships. It does not account for compounding macroeconomic factors (e.g., inflation), seasonal shifts outside of standard footfall, or the specific qualitative nature of the marketing campaigns being run. |
