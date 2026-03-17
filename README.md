# Overview
This project aims to predict whether a person is likely to have hypertension using structured health data.
Several machine learning models are trained and compared to identify the most effective approach, with special attention to performance in a medical context.

The goal is not only to maximize accuracy, but to understand how different models behave when detecting positive cases (hypertension), which is critical in real-world applications.

# Dataset

The dataset contains health and lifestyle variables such as:
- Age
- BMI
- Sleep duration
- Stress level
- Physical activity
- Dietary habits

Target variable:
- Hypertension Binary
  
# Methodology

The workflow follows a standard machine learning pipeline:

1. Data preprocessing
- Handling categorical variables (encoding)
- Feature scaling (StandardScaler / RobustScaler when needed)
- 
2. Train-test split
- Separation of training and testing data
- 
3. Model training
The following models were implemented:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree

4. Evaluation
Models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-score

Special focus is given to recall for the positive class, since missing a hypertension case is more critical than a false positive.

# Results

Each model shows different strengths:
- Logistic Regression: stable and interpretable baseline
- KNN: sensitive to feature scaling and data distribution
- Decision Tree: captures non-linear relationships and provides interpretability

The final model selection is based not only on accuracy but also on its ability to correctly identify hypertension cases.

# Tech Stack
- Python
- NumPy / Pandas
- Scikit-learn
- Matplotlib / Seaborn
