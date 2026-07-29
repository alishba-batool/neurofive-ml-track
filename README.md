# Titanic Survival Prediction using Logistic Regression

This project performs Exploratory Data Analysis (EDA), data preprocessing, feature engineering, and builds a Logistic Regression classification model to predict passenger survival on the Titanic dataset.

## Dataset

- **Dataset:** Titanic Dataset
- **Problem Type:** Binary Classification
- **Target Variable:** Survived
- **Language:** Python

## Libraries Used

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# Project Workflow

## 1. Data Exploration

- Loaded the Titanic dataset using Pandas
- Displayed the first five rows
- Checked dataset information
- Generated statistical summary
- Identified numerical and categorical columns
- Checked for missing values

---

## 2. Data Cleaning

- Filled missing values in the **Age** column using the median
- Filled missing values in the **Embarked** column using the mode
- Removed the **Cabin** column due to excessive missing values
- Removed unnecessary columns:
  - PassengerId
  - Name
  - Ticket

---

## 3. Data Visualization

- Visualized missing values
- Plotted Age Distribution (Histogram)
- Detected outliers using a Boxplot
- Created a Survival Count Plot
- Created a Correlation Heatmap
- Analyzed the relationship between Passenger Class and Survival

---

## 4. Feature Engineering

- Encoded categorical columns using **pd.get_dummies()**
- Converted categorical variables into numerical values suitable for machine learning

Encoded Columns:

- Sex
- Embarked

---

## 5. Model Building

A Logistic Regression model was trained to predict passenger survival.

Steps performed:

- Selected input features and target variable
- Split the dataset into training and testing sets using **train_test_split**
- Trained a Logistic Regression model
- Predicted survival on the test dataset

---

## 6. Model Evaluation

The model was evaluated using:

- Accuracy Score
- Confusion Matrix
- Classification Report

### Model Accuracy

**Accuracy:** **81.01%**

The Logistic Regression model correctly predicted passenger survival for approximately **81%** of the passengers in the test dataset.

---

## Confusion Matrix

The confusion matrix compares the model's predicted values with the actual values.

- True Positives represent passengers correctly predicted to have survived.
- True Negatives represent passengers correctly predicted not to have survived.
- False Positives represent passengers incorrectly predicted to have survived.
- False Negatives represent passengers incorrectly predicted not to have survived.

Most predictions fall along the diagonal of the confusion matrix, indicating good classification performance.

---

## Key Findings

- Most passengers were between **20 and 40 years** of age.
- The **Fare** column contains several outliers.
- First-class passengers had a significantly higher survival rate than third-class passengers.
- Passenger Class (**Pclass**) strongly influences survival.
- Female passengers had a higher survival rate than male passengers.
- Logistic Regression achieved an accuracy of **81.01%**, showing good predictive performance on the Titanic dataset.

---

## Requirements

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## Conclusion

This project demonstrates a complete machine learning workflow, starting with Exploratory Data Analysis (EDA), data cleaning, feature encoding, and visualization, followed by training and evaluating a Logistic Regression classification model.

The model achieved an accuracy of **81.01%**, indicating that Logistic Regression is an effective baseline algorithm for predicting Titanic passenger survival. This project provides a strong foundation for understanding data preprocessing, feature engineering, binary classification, and model evaluation using Scikit-learn.
