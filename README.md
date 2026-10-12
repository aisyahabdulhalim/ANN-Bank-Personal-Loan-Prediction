
# Brains Behind Banking: Predicting Customer Decisions with Artificial Neural Network (ANN)

An Artificial Neural Network (ANN) project to analyze bank customer data and predict personal loan status using machine learning.

## Project Overview

Banks need to identify customer characteristics associated with personal loan acquisition. This project uses an Artificial Neural Network (ANN) to learn patterns from customer data and predict loan status.

## Objectives

- Analyze bank customer characteristics.
- Perform Exploratory Data Analysis (EDA).
- Preprocess categorical and numerical data.
- Develop an ANN model using TensorFlow/Keras.
- Evaluate model performance using training and testing data.
- Investigate the model's ability to generalize to unseen data.

## Dataset Description

**Dataset:** UCI Bank Marketing Dataset  
**Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/222/bank+marketing)

| Attribute | Description |
|---|---|
| Number of Records | 4,521 |
| Number of Features | 16 |
| Related Features | 7 |
| Target Variable | `loan` |
| Problem Type | Binary Classification |

### Features

The dataset contains customer information such as:

- Age
- Job
- Marital status
- Education
- Account balance
- Housing loan status
- Personal loan status

### Target Distribution

- **84.72%:** Customers without a personal loan.
- **15.28%:** Customers with a personal loan.

The imbalanced class distribution is an important consideration during model evaluation.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow/Keras
- Jupyter Notebook

## Methodology

### 1. Data Collection

The dataset was imported from `bank.xlsx`.

### 2. Exploratory Data Analysis

- Examined the dataset structure.
- Analyzed customer loan status distribution.
- Visualized categorical and numerical features.
- Identified class imbalance.

### 3. Data Preprocessing

- Checked for missing values.
- Encoded categorical variables using ordinal encoding.
- Scaled numerical features.
- Prepared input features and target labels.

### 4. ANN Model Development

The neural network consists of:

- **Input Layer:** Receives the selected customer features.
- **Hidden Layers:** Learn patterns using ReLU activation.
- **Output Layer:** Uses sigmoid activation for binary classification.

### 5. Model Training

The dataset was divided into training and testing sets. The ANN was trained using TensorFlow/Keras, with training and validation performance monitored throughout the process.

### 6. Model Evaluation

The model was assessed using prediction plots, residual plots, and training-history visualizations.

Recommended classification metrics include:

- Accuracy
- Precision
- Confusion Matrix

## Results and Discussion

The project demonstrates how ANN can be applied to banking customer data.

Key observations:

1. The dataset contains an imbalanced distribution of loan status.
2. The ANN learns patterns from the training data.
3. Training and validation loss should be compared to identify potential overfitting.
4. Further tuning and evaluation are needed to assess generalization to unseen data.

## Future Improvements

- Tune ANN architecture and hyperparameters.
- Apply early stopping and regularization.
- Address class imbalance using class weights or resampling.
- Compare ANN with SVM and Random Forest.
- Evaluate using stratified cross-validation.
- Report precision, recall, F1-score, and ROC-AUC.
- Improve model generalization on unseen data.

## References

1. [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing)
2. [TensorFlow Documentation](https://www.tensorflow.org/)
3. [Keras Documentation](https://keras.io/)
4. [Bank Loan Project Resource](https://shayansoh.github.io/bankloan.html)

## 📄 License

This project was developed for educational and academic purposes. Refer to the original dataset source for applicable usage conditions.
