# Phishing Website Detection Using Machine Learning

## 1. Project Overview

Phishing Website Detection is a machine learning project that identifies whether a website URL is legitimate or phishing. It uses a Decision Tree Classifier to analyze numerical features from URLs and classify them into two categories.

The main goal is to help identify potentially dangerous websites and improve online security.

## 2. Project Title

**Phishing URL Detection Using Decision Tree Classifier**

## 3. Objectives

- Detect phishing URLs using machine learning.
- Classify URLs as legitimate or phishing.
- Train and test a Decision Tree Classifier.
- Evaluate model performance using standard metrics.
- Visualize the decision tree and confusion matrix.

## 4. Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

## 5. Dataset

**Dataset Name:** PhiUSIIL Phishing URL Dataset

The dataset contains URL-related features and a target column named `label`.

The model uses numerical features to predict whether a URL is legitimate or phishing.

**Target labels used in the code:**
- `0` — Legitimate
- `1` — Phishing

*Note: These mappings follow the intended target encoding in the code. Verify the dataset's original label definitions before interpreting the results.*

## 6. Project Workflow

### Step 1: Import Libraries

Import Pandas, NumPy, Matplotlib, and the required Scikit-learn modules.

### Step 2: Load the Dataset

Read the CSV dataset using Pandas and display its shape, first five rows, column names, missing values, and label counts.

### Step 3: Data Preprocessing

- Remove rows with missing target labels.
- Convert the target labels into binary values.
- Select numerical features.
- Replace infinite values with missing values.
- Fill missing feature values using their median.

### Step 4: Split the Dataset

Split the dataset into training and testing sets.

- Training data: 80%
- Testing data: 20%
- Random state: 42
- Stratification: Enabled

### Step 5: Train the Model

Train a Decision Tree Classifier using the following settings:

- Maximum depth: 5
- Class weight: Balanced
- Random state: 42

### Step 6: Visualize the Decision Tree

Display the trained decision tree to understand how the model makes its predictions.

### Step 7: Predict Results

Use the trained model to predict the labels of the testing data.

### Step 8: Generate the Confusion Matrix

Create a confusion matrix to compare actual labels with predicted labels.

### Step 9: Evaluate Model Performance

Calculate the following metrics:

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of predicted phishing URLs that are actually phishing.
- **Recall:** Proportion of actual phishing URLs correctly detected.
- **F1-score:** Balance between precision and recall.
- **Specificity:** Proportion of legitimate URLs correctly identified.

## 7. Model Evaluation

The model is evaluated using accuracy, precision, recall
