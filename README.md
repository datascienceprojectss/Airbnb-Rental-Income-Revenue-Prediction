# Airbnb-Rental-Income-Revenue-Prediction

Objective:

The project aimed to predict the success of Airbnb listings in London based on historical data, with "success" defined by revenue (price × number of reviews). The goal was to identify key factors driving rental income and provide actionable insights for hosts.

Key Steps:

Data Exploration

Datasets Used: Listings (property details), Reviews (customer feedback), and Neighborhoods (contextual data)

Findings:

Listings data had 75 columns with missing values.
Reviews data showed high user engagement (1.5M records).
Price distribution was right-skewed, with most listings priced low.
Apartments dominated the market.
Strong correlations between features like review_scores_communication and review_scores_location.

Feature Engineering:

Created a binary target variable ("Good"/"Bad") based on median revenue.
Normalized numerical features (price, reviews) to mitigate outliers.
Used one-hot encoding for categorical variables (e.g., property_type).

Modeling:

Algorithm: Random Forest Classifier (chosen for robustness and interpretability).
Training: 70-30 train-test split.

Results:

Accuracy: 78%.
F1-score: 0.78 (balanced precision/recall).
Key features: price_norm (86.6% importance), reviews_norm (13.4%).

Key Insights:

Pricing & Reviews Matter: Listings with competitive prices and moderate review activity were more likely to succeed.
Revenue as a Metric: While useful, revenue alone may overlook factors like guest satisfaction.
Model Strengths: Random Forest provided interpretable feature importance but had room for improvement.

Conclusion:

The project successfully identified pricing and review activity as key drivers of Airbnb listing success. The Random Forest model achieved decent accuracy (78%) and offered actionable insights for hosts. Future work could address data gaps and test advanced algorithms to refine predictions.

Final Note: This analysis bridges data science and business strategy, demonstrating how data-driven decisions can optimize rental income in the sharing economy.
