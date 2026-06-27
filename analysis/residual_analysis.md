# Residual Analysis & Predictive Variance

## Methodology
Residuals were calculated during the Multiple Regression execution. A residual is the difference between the **Actual Sales** a store achieved and the **Predicted Sales** the model calculated based on the equation: `Actual - Predicted = Residual`.

## Business Interpretation of Residuals
* **Largest Positive Residuals:** These are stores that significantly outperformed the model's expectations. If a store has a high positive residual, it means unmeasured factors; such as an exceptional store manager, localized viral trends, or superior visual merchandising are driving excess revenue. Leadership should audit these 5 stores to reverse-engineer their success.
* **Largest Negative Residuals:** These are stores that severely underperformed what their footfall, inventory, and location type dictated they should earn. High negative residuals indicate severe operational friction—poor staff training, local construction blocking access, or high theft rates. Leadership must intervene in these 5 locations immediately.

## Predictive Bias
By analyzing the scatter of residuals, the model appears highly accurate (82% variance explained), but leadership should manually monitor extreme edge cases (like ultra-high traffic holiday events), as linear regression models occasionally under-predict exponential spikes in consumer buying behavior.
