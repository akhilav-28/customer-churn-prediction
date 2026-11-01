# Customer Churn Prediction

## Project Overview
This project uses machine learning to predict whether a telecommunications customer is likely to leave the service (customer churn).

The goal is to identify customers at risk of leaving so that businesses can take proactive retention measures.

## Dataset
- **Dataset:** IBM Telco Customer Churn
- **Records:** 7,043 customers
- **Target variable:** `Churn`
- **Source:** [IBM Telco Customer Churn Dataset](https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv)

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Joblib
- Google Colab

## Project Workflow
1. Data loading and exploration
2. Data cleaning and preprocessing
3. Exploratory Data Analysis (EDA)
4. Feature encoding and scaling
5. Train-test split with stratification
6. Model training
7. Model evaluation
8. Hyperparameter tuning using GridSearchCV
9. Classification threshold comparison
10. Model saving and sample prediction

## Machine Learning Models
- Logistic Regression
- Random Forest Classifier
- Tuned Random Forest Classifier

## Model Performance

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 0.7381 | 0.5043 | 0.7834 | 0.6136 | 0.8413 |
| Random Forest | 0.7842 | 0.6224 | 0.4759 | 0.5394 | 0.8223 |
| Tuned Random Forest | 0.7395 | 0.5061 | 0.7781 | 0.6133 | 0.8398 |

Logistic Regression achieved the highest recall, F1 score, and ROC-AUC among the three evaluated models. Random Forest achieved the highest accuracy and precision.

## Classification Threshold
The Logistic Regression model was also evaluated at thresholds of 0.3, 0.4, 0.5, and 0.6.

A threshold of 0.5 achieved the highest F1 score in this comparison. Lower thresholds increased recall while reducing precision.

## Project Files
-  Customer_Churn_Prediction.ipynb` — Complete project notebook.
- `customer_churn_model.pkl` — Saved trained model and classification threshold (if uploaded).
- `requirements.txt` — Required Python libraries.

## How to Run
1. Open the notebook in Google Colab.
2. Run the cells from top to bottom.
3. The dataset is loaded directly from its source URL.
4. Review the model evaluation and sample prediction.

## Future Improvements
- Test additional classification algorithms.
- Perform more systematic hyperparameter tuning.
- Evaluate threshold selection using validation data.
- Deploy the model using a web application.

## Author
Akhil A V
MSc Computer Science (AI & ML)
