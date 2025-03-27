# 🚀 Credit Card Fraud Detection

## 📌 Overview
This project implements **Credit Card Fraud Detection** using **Machine Learning** techniques. The dataset is highly imbalanced, so techniques like **SMOTE** (Synthetic Minority Over-sampling) are used to improve fraud detection accuracy.

## 📂 Project Structure
- `data/` : Contains the dataset.
- `notebooks/` : Jupyter Notebooks for analysis and modeling.
- `src/` : Python scripts for preprocessing, feature engineering, and model training.
- `models/` : Saved trained models.
- `requirements.txt` : Dependencies required for running the project.

## 📊 Dataset Description
The dataset contains transaction records with the following key attributes:
- **Time**: Time elapsed between transactions.
- **Amount**: Transaction amount.
- **Class**: Target variable (0 = Normal, 1 = Fraud).

## 🛠️ Installation
To run this project locally, install the required dependencies:
```bash
# Clone the repository
git clone https://github.com/yourusername/CreditCard-FraudDetection.git
cd CreditCard-FraudDetection

# Install dependencies
pip install -r requirements.txt
```

## 🚀 Project Workflow
### **1️⃣ Data Preprocessing**
- Handling missing values
- Feature Engineering (Creating new features like transaction velocity)
- Data Scaling (StandardScaler applied to Amount & Time)

### **2️⃣ Handling Imbalance with SMOTE**
- Oversampling the minority class to improve fraud detection

### **3️⃣ Model Training & Evaluation**
- Models Used: Logistic Regression, Random Forest, XGBoost
- Metrics: **Accuracy, Precision, Recall, ROC-AUC Score**

## 📈 Results
- **Best Model**: Random Forest
- **ROC-AUC Score**: **0.98**
- **Key Observations**:
  - SMOTE improved fraud detection significantly.
  - Feature Engineering enhanced model accuracy.

## 💡 How to Use
Run the Jupyter Notebook:
```bash
jupyter notebook CreditCard-FraudDetection.ipynb
```
Modify hyperparameters in `src/model_training.py` to experiment with different models.

## 🔗 References
- [Kaggle Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- [SMOTE Explanation](https://imbalanced-learn.org/stable/over_sampling.html)

## 🤝 Contributing
Want to contribute? Feel free to fork the repo and submit pull requests!

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
