# 💳 Credit Card Fraud Detection

This project demonstrates how to detect fraudulent credit card transactions using machine learning techniques. The dataset is highly imbalanced, and the project includes techniques for handling such data, model training, and evaluation.

---

## 📂 Project Overview

This notebook-based project uses the **Credit Card Fraud Detection Dataset** containing anonymized transactions made by European cardholders in September 2013. The dataset contains:

- 284,807 transactions
- 492 fraudulent transactions (≈ 0.17%)

---

## 📊 Dataset Description

- `Time`: Seconds elapsed between a transaction and the first transaction in the dataset.
- `Amount`: Transaction amount.
- `V1` to `V28`: Principal components from PCA transformation (for confidentiality).
- `Class`: Target variable.  
  - `1` → Fraud  
  - `0` → Not Fraud

---

## ⚙️ Workflow

1. **Data Loading**
2. **Exploratory Data Analysis (EDA)**
3. **Handling Class Imbalance**
   - Using `RandomUnderSampler` to balance the data.
4. **Train-Test Split**
5. **Model Training**
   - Using `RandomForestClassifier`
6. **Evaluation**
   - Confusion Matrix
   - Precision, Recall, F1 Score
   - Area Under Precision-Recall Curve (AUPRC)

---

## 🧠 Machine Learning Techniques Used

- **Random Forest Classifier**  
  An ensemble learning method that builds multiple decision trees and merges them to get a more accurate and stable prediction.

- **Random Under-Sampling**  
  Balances the dataset by randomly removing samples from the majority class (non-fraud) to match the minority class (fraud). Useful in highly imbalanced datasets.

---

## 🧪 Evaluation Metrics

Why not use accuracy? Because:
- The dataset is **highly imbalanced**
- A model predicting everything as "Not Fraud" would still have 99.8% accuracy

Instead, we use:
- **Precision**
- **Recall**
- **F1 Score**
- **Area Under Precision-Recall Curve (AUPRC)**

---

## 🧰 Technologies and Libraries

- Python 3
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn

---

## 📁 File Structure

