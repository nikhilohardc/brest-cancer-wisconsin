# Breast Cancer Diagnosis Prediction with RandomForestClassifier

## Overview

This program performs breast cancer diagnosis prediction using machine learning techniques. It utilizes the Wisconsin Diagnostic Breast Cancer (WDBC) dataset to train a RandomForestClassifier model and make predictions on whether a tumor is malignant (M) or benign (B).

## Data

The dataset (`wdbc.csv`) contains various features related to tumor characteristics, such as radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimension. The target variable is 'diagnosis,' which is binary (1 for malignant, 0 for benign).

## Workflow

1. **Data Loading and Preprocessing:**
   - Load the dataset using Pandas.
   - Rename columns for clarity.
   - Drop unwanted columns, such as 'id.'
   - Map 'M' and 'B' in the 'diagnosis' column to 1 and 0, respectively.

2. **Data Exploration (EDA):**
   - Visualize the distribution of malignant and benign tumors.
   - Examine the correlation matrix heatmap to identify significant features.

3. **Train-Test Split:**
   - Split the dataset into training and testing sets.

4. **Model Building:**
   - Utilize RandomForestClassifier for breast cancer diagnosis prediction.
   - Utilize Logistic Regression for binary classification.
   - Evaluate the model using 10-fold cross-validation.