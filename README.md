# Customer Churn Prediction

## Objective

The goal of this project is to predict whether a customer will churn (leave) or stay with the company based on historical data. By identifying patterns and key factors that influence customer churn, businesses can take proactive measures to retain customers.

---

## Dataset

The dataset used in this project is available on Kaggle:  
[Kaggle Dataset Link](https://www.kaggle.com/datasets/shantanudhakadd/bank-customer-churn-prediction)

---

## Steps Taken

### 1. Data Preprocessing
- **Correlation Analysis:** Removed unnecessary columns after checking their correlation with the target variable (churn). This helped in reducing the complexity and focusing on relevant features.
- **Class Imbalance Handling:** Addressed the class imbalance issue by considering equal samples from both classes (churn vs. non-churn), ensuring a balanced dataset for training.

### 2. Feature Engineering
- **Label Encoding:** Applied label encoding to convert categorical variables into numerical format, making them suitable for model training.

### 3. Model Building
- **Logistic Regression:** Trained a Logistic Regression model to predict customer churn.
- **Gradient Boosting Classifier:** Used the Gradient Boosting Classifier for prediction, which is often effective in handling complex datasets.
- **Random Forest Classifier:** Built a Random Forest model for prediction. However, the Random Forest model showed signs of overfitting, especially when the number of trees was increased.

### 4. Model Evaluation
- **Comparison:** After training all three models (Logistic Regression, Gradient Boosting, and Random Forest), it was found that:
  - **Random Forest** showed signs of overfitting, performing well on training data but not generalizing well to test data.
  - **Logistic Regression** and **Gradient Boosting** performed similarly, with identical accuracy scores.
- **Final Model:** Chose the **Gradient Boosting Classifier** for the final prediction due to its robust performance and ability to handle imbalanced data.

---

## Kaggle Notebook

You can find the complete code implementation and analysis in my Kaggle notebook:  
[Kaggle Notebook Link](https://www.kaggle.com/code/varshithpsingh/customer-churn-prediction)

---

## Insights and Results

- **Random Forest** overfitted the data, leading to a significant drop in performance on test data.
- **Logistic Regression** and **Gradient Boosting** produced similar accuracy, with **Gradient Boosting** selected for the final model.
- The Gradient Boosting model successfully predicted customer churn, providing valuable insights for improving customer retention strategies.
