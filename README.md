# Homeownership-Prediction-using-SVM

This project uses Support Vector Machines (SVM) to analyze socioeconomic factors influencing homeownership status in Washington State. By training linear, radial, and polynomial SVM models, the analysis seeks to predict whether a home is owned or rented based on features like age, income, education, and household size.

## Project Overview

- **Dataset**: U.S. Census data from Washington State, containing 24 variables on 30,802 unique households.
- **Objective**: Predict homeownership status (owned/rented) and identify key factors impacting ownership likelihood.
- **Models**:
  - **Linear SVM**: Suitable for linearly separable data, reaching 82.6% accuracy.
  - **Radial SVM**: Captures non-linear relationships, achieving up to 82.8% accuracy after tuning.
  - **Polynomial SVM**: Best-performing model with up to 83.1% accuracy for non-linear separable data.

## Key Features

1. **Data Cleaning and Preprocessing**:
   - Aggregated household data to create unique entries, filtered relevant features, and encoded categorical variables.
   - Processed variables such as marital status, education level, and income for effective SVM model input.

2. **Model Tuning and Optimization**:
   - Used Grid Search with cross-validation to optimize parameters (C, gamma, degree) for each model.
   - Identified best-fit parameters for improved prediction accuracy and reliability.

3. **Feature Importance and Visualization**:
   - Analyzed decision boundaries and feature importance to understand the influence of factors like age and household income.
   - Created visualizations to highlight key trends and aid in interpreting model outputs.

## Results

- **Linear SVM Model**: Achieved 82.6% accuracy with optimal C value.
- **Radial SVM Model**: Achieved 82.8% accuracy with optimized C and gamma values.
- **Polynomial SVM Model**: Achieved the highest accuracy of 83.1% with optimized C and degree values.

## Getting Started

1. **Install Dependencies**: Required libraries include `scikit-learn`, `pandas`, `matplotlib`.
2. **Data Preparation**: Follow `data_preprocessing.py` to clean and preprocess the data.
3. **Model Training and Evaluation**: Run `svm_model_training.py` to train each SVM model, followed by `model_evaluation.py` for testing.

## Conclusion

This project provides insights into factors affecting homeownership, supporting data-driven strategies for policy-making. Key features influencing ownership status include income, age, and marital status, with polynomial SVM proving most effective in prediction.

## Future Enhancements

- Experiment with other classification algorithms for comparison.
- Expand to other socioeconomic datasets for broader insights.
- Refine feature engineering for improved model performance.

---

This project leverages machine learning for meaningful insights into housing data, with applications for policymakers and prospective homeowners.
