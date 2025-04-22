# 🛡️ Credit Card Fraud Detection using Logistic Regression

This project demonstrates how to detect fraudulent credit card transactions using a **logistic regression model**. It leverages a real-world dataset and applies classic data preprocessing and machine learning techniques to build a binary classification model.

---

## 📁 Dataset

The dataset used in this project is from [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud), which contains transactions made by European cardholders in September 2013. It includes:

- Features are numerical results of PCA transformations, except `Time` and `Amount`
- The target variable is `Class`:  
  - `0` = Legitimate  
  - `1` = Fraudulent

---

## ⚙️ Project Workflow

1. **Data Exploration & Preprocessing**
   - Checked for missing values
   - Analyzed class imbalance
   - Sampled a balanced dataset by undersampling legitimate transactions

2. **Feature Scaling**
   - Applied `StandardScaler` to normalize input features

3. **Model Training**
   - Used **Logistic Regression** (`solver='saga'`, `max_iter=1000`)
   - Trained on 80% of the balanced dataset

4. **Evaluation**
   - Evaluated using accuracy on training and testing data
   - Future improvements could include precision, recall, F1 score, or ROC-AUC

---

## 📊 Results

- Achieved high accuracy on both training and testing datasets
- Demonstrates how logistic regression can serve as a strong baseline for binary fraud detection tasks

---

## 🧰 Tech Stack

- Python
- Jupyter Notebook
- NumPy & Pandas
- Scikit-learn

---

## 🚀 Getting Started

1. Clone this repository  
   ```bash
   git clone https://github.com/yourusername/credit-card-fraud-detection.git
   ```

2. Install dependencies  
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook  
   Open `credit_card.ipynb` in Jupyter or VS Code.

---

## ✅ To Do

- Add precision, recall, F1-score metrics
- Try other models (Random Forest, XGBoost, etc.)
- Handle full dataset with SMOTE or ensemble methods


