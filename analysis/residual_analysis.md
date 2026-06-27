# Residual Analysis & Predictive Variance

## 1. Methodology
Residuals were calculated during the Multiple Regression execution. A residual represents the difference between the **Actual Sales** a store achieved and the **Predicted Sales** the model calculated based on our equation (`Actual - Predicted = Residual`). 

## 2. Residual Outliers Identified
By sorting the residual output to find the extreme variances across the entire dataset, the following anomalies were identified:

**Top 5 Largest Positive Residuals (Outperformers):**
1. **Observation #888:** +$105,658.90
2. **Observation #728:** +$102,434.30
3. **Observation #578:** +$83,526.19
4. **Observation #633:** +$83,307.72
5. **Observation #163:** +$78,378.11

**Top 5 Largest Negative Residuals (Underperformers):**
1. **Observation #158:** -$66,742.66
2. **Observation #391:** -$57,211.52
3. **Observation #894:** -$52,060.04
4. **Observation #632:** -$50,916.14
5. **Observation #987:** -$50,490.87

## 3. Business Interpretation
* **Positive Residuals:** These are stores that significantly outperformed the model's mathematical expectations. For example, Observation #888 generated over $105k more than its footfall, inventory, and location type dictated. This indicates unmeasured positive factors—such as an exceptional store manager, localized viral trends, or superior visual merchandising. Leadership should audit these specific top 5 stores to reverse-engineer and scale their success.
* **Negative Residuals:** These are stores that severely underperformed. Observation #158 fell $66k short of expectations. High negative residuals indicate severe operational friction not captured by the data—poor staff training, local construction blocking physical access, or high theft rates. Leadership must intervene in these bottom 5 locations immediately to stop the bleeding.

## 4. Predictive Bias
By analyzing the scatter of residuals, the model appears highly accurate (82% variance explained). However, the existence of six-figure positive residuals proves that leadership should manually monitor extreme edge cases (like ultra-high traffic holiday events or localized anomalies), as linear regression models will structurally under-predict exponential spikes in consumer buying behavior.
