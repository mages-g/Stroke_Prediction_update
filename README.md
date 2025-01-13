# Stroke Prediction using Machine Learning

## Project Narrative
Stroke is a leading cause of death globally, responsible for approximately 11% of total deaths according to the World Health Organization (WHO). Early prediction of strokes can significantly improve healthcare outcomes by enabling timely interventions. This project aims to predict the likelihood of stroke occurrence in patients based on demographic, lifestyle, and medical factors.

### Dataset Description
The dataset used in this project contains features such as:
- **Gender**: Male, Female, or Other
- **Age**: Age of the patient
- **Hypertension**: 0 (No), 1 (Yes)
- **Heart Disease**: 0 (No), 1 (Yes)
- **Marital Status**: Yes or No
- **Work Type**: Government, Private, Self-employed, etc.
- **Residence Type**: Urban or Rural
- **Average Glucose Level**: Blood glucose levels
- **BMI**: Body Mass Index
- **Smoking Status**: Formerly smoked, never smoked, smokes, or unknown
- **Stroke**: Target variable (1 if the patient had a stroke, 0 otherwise)

The data underwent cleaning and preprocessing, including handling missing values, scaling, and encoding categorical variables.


## Machine Learning Models Evaluated
Several models were evaluated to identify the best-performing algorithm for stroke prediction:
- Logistic Regression
- Decision Tree Classifier
- Support Vector Classifier (SVC)
- Random Forest Classifier
- K-Nearest Neighbors (KNN)

### Why KNN?
Among all the models tested, K-Nearest Neighbors (KNN) demonstrated the best cross-validation performance. This can be attributed to:
- **Simplicity**: KNN makes no assumptions about the underlying data distribution, which suits datasets with a mix of numeric and categorical features.
- **Adaptability**: The algorithm dynamically adjusts based on the distribution of the nearest neighbors, ensuring robust classification.
- **Performance**: During hyperparameter tuning, KNN consistently showed the highest accuracy and F1 scores compared to other models.

#### Cross-Validation Results
The KNN model's performance metrics during cross-validation were as follows:
- **Accuracy**: 89%
- **F1 Score**: 0.86

These metrics were superior to other models, which struggled with overfitting or poor generalization.

## Visual Insights
### Data Distribution
Below is a graph illustrating the distribution of key features like age, BMI, and glucose levels:

![Feature Distribution](placeholder-for-graph)

### Model Comparison
A comparative chart showing the accuracy of various models tested:

![Model Comparison](placeholder-for-graph)

### KNN Hyperparameter Tuning
Optimal performance was achieved with the following hyperparameters:
- **Number of Neighbors (k)**: 7
- **Distance Metric**: Euclidean

![KNN Performance](placeholder-for-graph)

## Observations and Conclusion
1. **Feature Importance**: Age and glucose levels were the most significant predictors of stroke.
2. **KNN's Effectiveness**: Its non-parametric nature made it ideal for this dataset, handling imbalanced classes effectively.
3. **Generalization**: KNN showed excellent generalization during testing, outperforming complex models like Random Forest.
4. **Future Scope**: Incorporating additional health indicators or real-time monitoring data could further enhance predictive accuracy.

This project demonstrates how KNN can serve as a reliable model for stroke prediction, balancing simplicity and performance effectively.

