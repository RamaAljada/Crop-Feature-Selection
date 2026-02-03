# Crop-Feature-Selection
A machine learning project to identify the most important soil feature for crop prediction using Logistic Regression.
The project successfully achieves Feature Selection

A farmer wanted to know which soil feature is the most important to predict the best crop for his field. Available features were: Nitrogen (N), Phosphorus (P), Potassium (K), and pH
The project aimed to use Feature Selection to find the most influential feature and help the farmer make data-driven decisions.

## Tools
- Programming language: Python
- Libraries:
  - pandas → data manipulation and exploration
  - scikit-learn → Logistic Regression, train_test_split, accuracy_score, StandardScaler
  - matplotlib → visualizing distributions and results

## Workflow
1. Plot histograms for each feature to understand distributions and detect outliers
2. Apply StandardScaler to numerical features (N, P, K, ph) to normalize scales
3. Train Logistic Regression on each feature individually and calculate accuracy
4. Compare results to determine the best predictive feature

## Results
Feature scores after scaling:
{'N': 0.15, 'P': 0.166, 'K': 0.245, 'ph': 0.098}
Best predictive feature: K (Potassium)

## Conclusion
- K (Potassium) is the most important feature for crop prediction
- N and P have medium influence, pH has the least
- The farmer can focus on measuring potassium to select the most suitable crops
- Workflow is clear: Distribution analysis → Scaling → Model training → Best feature selection
