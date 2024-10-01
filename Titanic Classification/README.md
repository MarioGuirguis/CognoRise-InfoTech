# Titanic Survival Prediction

This project utilizes the Titanic dataset to construct a machine learning model that predicts whether a passenger survived the Titanic disaster. The goal is to apply data science techniques to gain insights into the survival patterns among the passengers and create an accurate predictive model.

## Overview of the Code

This Jupyter notebook implements a machine learning pipeline to predict the survival of Titanic passengers. It follows these key steps:

1. **Data Loading and Exploration:**
   - The Titanic dataset is loaded, and a preview of the data is displayed.
   - Missing values are filled with appropriate replacements, such as zeros for missing values in `Cabin`.

2. **Data Preprocessing:**
   - The dataset is prepared by filling missing values and converting categorical features (`Sex` and `Embarked`) into numeric form.
   - The dataset is split into training and testing sets to train the model and evaluate its performance.

3. **Model Training:**
   - Support Vector Machine (SVM) is used to train a model based on the prepared data.
   - The model is fit on the training data and predicts outcomes on the test set.

4. **Model Evaluation:**
   - The model's accuracy is calculated by comparing the predictions with the actual survival outcomes in the test set.
   - The notebook outputs an accuracy of approximately 98.81%.
