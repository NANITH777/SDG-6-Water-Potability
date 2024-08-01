### Water Potability Prediction Project

#### Goal

The goal of this project is to develop a machine learning model to predict the potability of water based on its chemical properties. By analyzing and preprocessing the data, and applying different machine learning algorithms with hyperparameter tuning, the best performing model is selected to make reliable predictions on water quality. The final model is then saved for future use.

This project is part of a `Hackathon` organized by the <strong> Frontier Tech Leaders </strong> community, aiming to contribute solutions to the United Nations' Sustainable Development Goals (SDG), particularly focusing on ensuring clean water and sanitation for all.

#### Steps Involved

1. **Data Loading and Exploration**

   - Loaded the dataset.
   - Displayed initial information, including the first and last few rows, column names, and data types.
   - Checked for missing values and the distribution of the target variable ('Potability').

2. **Data Cleaning and Preprocessing**

   - Filled missing values in critical columns ('ph', 'Sulfate', 'Trihalomethanes') with their median values.
   - Saved the cleaned data to a new CSV file.
   - Normalized the data to scale features to a range of 0 to 1 for better model performance.

3. **Data Visualization**

   - Visualized relationships between features using pairplots, bar plots, box plots, and violin plots.
   - Created a correlation heatmap to understand the relationships between numerical features.
   - Categorized pH values into intervals and visualized their distribution.

4. **Feature Engineering**

   - Extracted feature importances from a Decision Tree model to understand which features are most influential in predicting water potability.
   - Plotted the feature importances and visualized the decision tree.

5. **Model Training and Hyperparameter Tuning**

   - Split the data into training and testing sets.
   - Defined different models (Random Forest, Logistic Regression, Decision Tree, SVM) and their respective hyperparameters for tuning.
   - Performed hyperparameter tuning using `GridSearchCV` to find the best model and parameters.
   - Selected the model with the highest cross-validated score (Random Forest in this case).

6. **Model Evaluation**

   - Trained the final model with the best parameters on the training data.
   - Evaluated the model on the test set using accuracy, precision, recall, F1 score, and a classification report.
   - Visualized the confusion matrix to understand the performance of the model in terms of true positives, true negatives, false positives, and false negatives.

7. **Model Deployment**
   - Saved the trained model using `joblib` for future use in making predictions.
   - Demonstrated making predictions on new data.
