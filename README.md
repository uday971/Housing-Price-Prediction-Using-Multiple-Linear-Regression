# Housing-Price-Prediction-Using-Multiple-Linear-Regression
A complete, end-to-end multiple-linear-regression (MLR) workflow that turns raw housing listings into an explainable pricing engine. Starting with a 13-column CSV (area, bedrooms, bathrooms, amenities, etc.), the pipeline:

1. Loads & inspects data with pandas, revealing numeric vs. categorical attributes and basic summary stats.

2. Visual-explores relationships (scatter, box-plots, correlation heat-map) to spot the strongest price drivers and potential outliers.

3. Encodes categorical amenities (yes/no → 0/1; furnishing status → ordinal codes) for model readiness.

4. Diagnoses multicollinearity with the Variance Inflation Factor, then drops the lone high-VIF feature to stabilize coefficients.

5. Fits an OLS regression in statsmodels, producing clean, business-friendly coefficients—e.g., every additional bathroom adds roughly ₹1 million; central A/C adds ~₹0.85 million.
6. Package insights in a concise slide deck and plots ready for stakeholders.

Key findings
* Area and bathrooms dominate the price influence, followed by the number of stories and amenity flags, such as basement and air conditioning.
* Upgrades pay off differently: indoor comforts (A/C, hot-water heating) and extra parking slots yield stronger premiums than cosmetic furnishing status.
* Model explainability first: by taming multicollinearity and keeping the feature set lean, each coefficient reads as a straightforward cash increment—perfect for broker negotiations.
