💳 Credit Card Fraud Detection using Machine Learning

📌 Project Overview

Credit card fraud is one of the biggest challenges faced by financial institutions. Fraudulent transactions lead to significant financial losses and negatively impact customer trust. This project develops a machine learning model to identify fraudulent credit card transactions using historical transaction data.

The dataset contains anonymized credit card transactions made by European cardholders over two days in September 2013. Due to confidentiality, the original features were transformed using Principal Component Analysis (PCA).

The objective is to accurately classify fraudulent transactions while handling the severe class imbalance present in the dataset.

🎯 Business Problem

Financial institutions need an efficient fraud detection system that can:

- Detect fraudulent transactions quickly
- Minimize financial losses
- Reduce false positives
- Improve customer experience
- Support real-time fraud prevention

📊 Dataset

Source: European Credit Card Fraud Detection Dataset

- Total Transactions: **284,807**
- Fraudulent Transactions: **492**
- Genuine Transactions: **284,315**
- Fraud Rate: **0.172%**

Features

| Feature | Description |
|----------|-------------|
| Time | Seconds elapsed between transactions |
| V1–V28 | PCA transformed numerical features |
| Amount | Transaction amount |
| Class | Target variable (0 = Genuine, 1 = Fraud) |

🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- imbalanced-learn (SMOTE)
- SciPy

📂 Project Workflow

1. Data Collection

- Loaded transaction dataset
- Inspected dataset structure
- Verified feature types

2. Data Cleaning

- Checked for missing values
- Verified data quality
- Confirmed no duplicate handling required

3. Exploratory Data Analysis (EDA)

Performed:

- Summary statistics
- Distribution analysis
- Fraud vs Non-Fraud comparison
- Transaction amount analysis
- Transaction time analysis
- Correlation analysis
- Class imbalance visualization

4. Statistical Analysis

Conducted:

- Shapiro-Wilk Normality Test
- Mann-Whitney U Test

Key Findings:

- Dataset is not normally distributed.
- Fraudulent transactions exhibit different temporal patterns than genuine transactions.

5. Data Preprocessing

- Feature selection
- Train-Test Split
- SMOTE oversampling to balance the minority class

6. Machine Learning

Implemented:

- Random Forest Classifier

Model training included:

- Model fitting
- Prediction
- Performance evaluation

📈 Model Evaluation

Metrics evaluated:

- Accuracy
- Confusion Matrix

Results
- Training Accuracy: 100%
- Testing Accuracy : 99.99%

Note: Since this is an imbalanced classification problem, metrics such as Precision, Recall, F1-Score, ROC-AUC, and Precision-Recall AUC are recommended for production-grade evaluation.

📊 Visualizations

The project includes visualizations for:

- Transaction distribution
- Fraud vs Genuine transactions
- Transaction amount comparison
- Time distribution
- Feature distributions
- Correlation heatmap
- Class imbalance
- SMOTE balanced dataset

📁 Project Structure

Credit-Card-Fraud-Detection/
│
├── data/
│   └── creditcard.csv
│
├── notebooks/
│   └── Fraud_Detection.ipynb
│
├── images/
│
├── README.md
│
└── requirements.txt

🚀 Future Improvements
- Implement XGBoost and LightGBM
- Hyperparameter tuning using GridSearchCV
- Cross-validation
- SHAP Explainability
- Precision-Recall Curve
- ROC Curve
- Cost-sensitive learning
- Threshold optimization
- Real-time fraud detection API using Flask
- Docker deployment
- AWS deployment

💡 Business Impact

This project demonstrates how machine learning can help financial institutions:

- Detect fraudulent transactions faster
- Reduce operational losses
- Improve customer trust
- Support automated fraud investigation
- Enhance transaction monitoring

📚 Learning Outcomes

- Data Cleaning
- Exploratory Data Analysis
- Statistical Testing
- Handling Imbalanced Data
- Feature Engineering
- Machine Learning Classification
- Model Evaluation
- Data Visualization
- Business Problem Solving

