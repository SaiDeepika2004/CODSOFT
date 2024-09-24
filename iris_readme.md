# Iris Flower Detection with Random Forest

![image](https://github.com/user-attachments/assets/5fb89d11-0ef0-49e5-9a1d-a79651ff2a60)

## Table of Contents
- [Project Overview](#project-overview)
- [Business Understanding](#business-understanding)
- [Objectives](#objectives)
- [Data Understanding](#data-understanding)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Modeling](#modeling)
- [Hyperparameter Tuning](#hyperparameter-tuning)
- [Cross-Validation](#cross-validation)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)
- [Next Steps](#next-steps)

## Project Overview
The **Iris Flower Detection** project involves building a machine learning model to classify iris flower species based on four key features: sepal length, sepal width, petal length, and petal width. This project utilizes the **Random Forest** algorithm, further enhanced by hyperparameter tuning and cross-validation to improve model accuracy.

## Business Understanding
The correct classification of iris flower species can assist in scientific research and educational purposes, providing a framework for understanding basic classification problems in machine learning. Reliable species identification is crucial for botany, taxonomy, and even biological studies.

## Objectives
- **Predict Iris Species**: Build a machine learning model to accurately predict the species of an iris flower based on input features.
- **Model Optimization**: Implement hyperparameter tuning and cross-validation to optimize the performance of the Random Forest model.
- **Feature Importance**: Identify the most important features in determining the iris species.
- **Provide Insights**: Offer actionable insights from the model that can benefit both educational and scientific communities.

## Data Understanding
The dataset used for this project is from Kaggle: [Iris Species Dataset](https://www.kaggle.com/uciml/iris).

### Key Columns:
- `SepalLengthCm`: Length of the sepal in centimeters
- `SepalWidthCm`: Width of the sepal in centimeters
- `PetalLengthCm`: Length of the petal in centimeters
- `PetalWidthCm`: Width of the petal in centimeters
- `Species`: The target variable (Setosa, Versicolor, or Virginica)

### Dataset Summary:
- **150 Instances**: The dataset contains 150 records, 50 for each species.
- **No Missing Data**: There are no missing or null values in the dataset.

## Exploratory Data Analysis (EDA)
Key insights from the EDA include:
- **Species Distribution**: The dataset is balanced, with each species having equal representation.
- **Feature Correlations**: Petal length and petal width have the strongest correlation with species classification.
- **Sepal and Petal Size Analysis**: Versicolor species show moderate values for both sepal and petal size, while Setosa has smaller petal dimensions and Virginica shows the largest petal dimensions.

## Modeling
For this project, the **Random Forest Classifier** was chosen due to its robustness, ability to handle complex data relationships, and low risk of overfitting.

### Model Implementation:
1. **Baseline Model**: Random Forest Classifier without hyperparameter tuning.
2. **Model Evaluation**: Accuracy, precision, recall, and F1-score were used to assess the model's performance.

### Key Features:
The most important features in predicting iris species:
- **Petal Length**: The most influential feature.
- **Petal Width**: Second in importance for species classification.
- **Sepal Length and Width**: Less impactful but still relevant.

## Hyperparameter Tuning
Hyperparameter tuning was performed using Grid Search to identify the optimal parameters for the Random Forest model. The following parameters were tuned:
- **n_estimators**: Number of trees in the forest.
- **max_depth**: Maximum depth of the trees.
- **min_samples_split**: Minimum number of samples required to split a node.
- **min_samples_leaf**: Minimum number of samples required to be at a leaf node.

After tuning, the best hyperparameters were:
- `n_estimators = 100`
- `max_depth = 5`
- `min_samples_split = 3`
- `min_samples_leaf = 1`

## Cross-Validation
Cross-validation was used to validate the stability and generalization of the model. Using 10-fold cross-validation, the average accuracy across all folds was **97%**, demonstrating the model's reliability and performance consistency.

## Recommendations
- **Petal Features**: Focus on the petal length and width for species classification, as they provide the most predictive power.
- **Model Performance**: The tuned Random Forest model provides excellent classification results and can be used for future tasks involving iris species detection.
- **Educational Use**: This model serves as a great example for understanding classification techniques and the importance of hyperparameter tuning in machine learning projects.
  
## Conclusion
The Iris Flower Detection project successfully classified iris species using a Random Forest model optimized through hyperparameter tuning and cross-validation. The petal length and width were found to be the most important features. This project showcases how data-driven insights can aid in educational and biological research.

## Next Steps
- **Incorporate New Features**: Investigate additional biological factors that may improve classification accuracy.
- **Test Other Models**: Explore different machine learning models such as SVM or Gradient Boosting for further comparison.
- **Real-time Classification**: Build a real-time classification app using the trained model for practical use in educational settings.
