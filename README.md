
# Customer Churn Analysis

This project focuses on predicting customer churn using supervised machine learning models.  
It walks through data preprocessing, exploratory data analysis, model training, and evaluation using both unbalanced and SMOTE-balanced datasets.

## Dataset

The dataset contains customer data and a binary churn label.  
It includes categorical and numerical features such as:

- Contract type
- Tenure
- Monthly charges
- Payment method
- Internet service
- Senior citizen status

## Project Steps

1. **Data Cleaning & Preprocessing**
   - Handled missing values
   - One-hot encoded categorical features
   - Scaled numerical features with StandardScaler

2. **Exploratory Data Analysis (EDA)**
   - Analyzed churn distribution (~26% churn rate)
   - Correlation matrix and bar/pie charts to identify patterns

3. **Handling Class Imbalance**
   - Applied SMOTE to balance the training data
   - Compared model performance on original vs. SMOTE-balanced data

4. **Models Trained**
   - Logistic Regression
   - Random Forest
   - XGBoost

   Each model was trained on:
   - Unbalanced data
   - SMOTE-balanced data

5. **Evaluation Metrics**
   - Accuracy, Precision, Recall, F1-score
   - Confusion matrix
   - KDE plots (Actual vs Predicted distributions)

6. **Model Comparison**
   - Results were collected and visualized using grouped bar plots
   - Key focus was on **Recall**, due to the cost of missing churners

## Key Takeaways

- Logistic Regression improved recall significantly with SMOTE, but at a cost to precision.
- Random Forest performed very well in terms of recall without SMOTE.
- XGBoost offered a good balance between recall and precision, especially with SMOTE.

## Files

- `CustomerChurnAnalysis.ipynb` – full notebook with code, analysis, and results
- `README.md` – project summary and instructions
- `requirements.txt` - list of Python packages required to run the notebook

## Requirements

- Python 3.8+
- pandas, matplotlib, seaborn
- scikit-learn
- imbalanced-learn
- xgboost


## How to run
1. Clone the repository and install dependencies:

```bash
git clone https://github.com/jacek-kozakowski/customer-churn-analysis.git
cd customer-churn-analysis
pip install -r requirements.txt
```

2. Navigate to project directory and open the notebook:

```bash
jupyter notebook CustomerChurnAnalysis.ipynb
```
## Author

**Jacek Kozakowski** – [LinkedIn][https://www.linkedin.com/in/jacek-kozakowski-31b759356/]
