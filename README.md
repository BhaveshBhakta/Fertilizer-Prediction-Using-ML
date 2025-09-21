## Fertilizer Prediction

### Project Overview

This project aims to predict the **appropriate fertilizer for a specific crop** based on soil and climate conditions. By analyzing features such as temperature, humidity, moisture, soil type, crop type, and nutrient levels (Nitrogen, Potassium, Phosphorous), the goal is to develop a machine learning model that can recommend the most suitable fertilizer. This is a practical application in precision agriculture to maximize crop yield and minimize waste.

-----

### Technical Highlights

  * **Dataset**: [Kaggle - Fertilizer Prediction](https://www.kaggle.com/datasets/gdabhishek/fertilizer-prediction)
  * **Size**: 99 entries, 9 columns.
  * **Key Features**:
      * **Environmental**: `Temparature`, `Humidity`, `Moisture`.
      * **Soil & Crop**: `Soil Type`, `Crop Type`.
      * **Nutrients**: `Nitrogen`, `Potassium`, `Phosphorous`.
  * **Approach**:
      * **Data Cleaning**: The dataset was clean with no missing values or duplicates.
      * **Exploratory Data Analysis**: Histograms, box plots, bar charts, and scatter plots were used for visualization to understand data distributions and feature relationships.
      * **Label Encoding**: Applied to all categorical features (`Soil Type`, `Crop Type`) and the target `Fertilizer Name`.
      * **Multi-class Classification**: The target variable `Fertilizer Name` has 7 distinct categories.
      * **Models Used**:
          * Logistic Regression, Ridge Classifier, SVC, Random Forest, XGBoost, AdaBoost, Gradient Boosting, Bagging, Decision Tree.
  * **Best Accuracy**:
      * **100%** with Logistic Regression, XGBoost, Bagging, and Decision Tree Classifiers.
      * **95.0%** with Random Forest and Gradient Boosting Classifiers.
      * The extremely high accuracies for multiple models on this small dataset suggest a very strong relationship between the input features and the recommended fertilizer.

-----

### Purpose and Applications

  * Enable farmers to **select the most appropriate fertilizer** for their crops and soil conditions.
  * Optimize nutrient application, leading to healthier plants and higher crop yields.
  * Reduce the environmental impact of agriculture by preventing over-fertilization.
  * Provide a foundational model for smart farming and precision agriculture systems.

-----

### Installation

Clone the repository and download the dataset.

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost
```

-----

### Collaboration

We welcome contributions to improve the project. You can help by:

  * Investigating the very high accuracy for potential data leakage or an overly simple classification task.
  * Performing comprehensive hyperparameter tuning and cross-validation for all models to ensure robustness.
  * Exploring more advanced feature engineering techniques.
  * Adding explainability (e.g., SHAP or LIME) to understand which soil and climate factors are the most critical for recommending a specific fertilizer.
