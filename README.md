### Parkinson's Disease Prediction

**Overview**

This project focuses on developing a machine learning model to predict Parkinson's disease. We employ a Support Vector Machine (SVM) classifier, trained on a dataset encompassing various vocal features, to discriminate between individuals with and without Parkinson's.

**Dependencies**

Essential Python libraries for this project include:

-   numpy
-   pandas
-   scikit-learn

To install these libraries, use pip:

Bash

```
pip install numpy pandas scikit-learn

```

Use code [with caution.](/faq#coding)

**Data Collection and Analysis**

The dataset, stored in `parkinsons.csv`, comprises 195 rows and 24 columns. Data points represent vocal attributes, and the target variable indicates Parkinson's status (1: positive, 0: healthy).

**Data Analysis Summary:**

-   No missing values detected.
-   Statistical summary generated (mean, standard deviation, etc.).
-   Class imbalance observed: 147 Parkinson's cases, 48 healthy controls.

**Data Preprocessing**

The preprocessing steps involve:

-   Loading the dataset using Pandas.
-   Inspecting data for missing values and generating statistical summaries.
-   Isolating features and the target variable.
-   Partitioning data into training and testing sets.
-   Standardizing features to achieve zero mean and unit variance.

**Model Training**

An SVM model with a linear kernel is employed. The model is trained on the prepared training data.

**Model Evaluation**

The trained model demonstrates:

-   Training accuracy of 88.46%
-   Testing accuracy of 87.18%

**Predictive System**

A basic prediction system is implemented to classify new instances based on the trained model. The output categorizes individuals as either having or not having Parkinson's disease.

Python

```
prediction = model.predict(std_data)
print(prediction)
if (prediction[0] == 0):
    print("The Person does not have Parkinson's Disease")
else:
    print("The Person has Parkinson's Disease")   1. github.com github.com
```
