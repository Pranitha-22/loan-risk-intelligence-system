# 🏦 Loan Approval Prediction System (India)

This project is an end-to-end Machine Learning system built in Google Colab that predicts loan approval and classifies applicants into risk categories using real-world banking data.

---

## 🚀 Features

- Loan approval prediction using ML models  
- Risk classification (Low / Medium / High)  
- Feature engineering (Total Income, log transformations)  
- Model evaluation (Accuracy, ROC-AUC, Precision, Recall)  
- Explainable AI using SHAP  
- Streamlit app for real-time prediction  

---

## 🧠 ML Pipeline

Data → Cleaning → Feature Engineering → Encoding → Scaling → Model Training → Evaluation → SHAP → Risk Segmentation → Deployment  

---

## 📊 Model Performance

- Accuracy: ~85%  
- ROC-AUC: ~0.84  
- Recall (Approved): ~0.98  
- Recall (Rejected): ~0.58  

---

## 🧠 Explainable AI (SHAP)

To make the model transparent and interpretable, SHAP (SHapley Additive Explanations) was used.

- Identifies feature contributions to predictions  
- Explains both global model behavior and individual predictions  
- Improves trust in model decisions (important in financial applications)  

### Key Insights:
- Credit_History is the most influential feature  
- Higher income increases approval probability  
- Larger loan amounts can negatively impact approval  

SHAP transforms the model from a black-box into an explainable decision system.

---

## 🔍 Key Insights (Train Data)

- Credit History is the most important feature  
- Income alone is not sufficient for loan approval  
- Feature engineering improved model performance  
- Semi-urban applicants have higher approval rates  
- Dataset has slight class imbalance  

---

## 📊 Test Data Insights

- Total applicants: 367  
- Missing values handled using mode (categorical) and median (numerical)  

### Observations:
- Income is right-skewed (most between ₹2K–₹6K)  
- Loan amount mostly between 100–150  
- Majority applicants are from urban/semi-urban areas  
- Most applicants have valid credit history  

---

## 📈 Prediction Results

- Approved: 306 (~83%)  
- Rejected: 61 (~17%)  

---

## 🚦 Risk Classification

- Low Risk → probability > 0.75  
- Medium Risk → 0.4 – 0.75  
- High Risk → < 0.4  

| Risk Level   | Count |
|-------------|------|
| Low Risk    | 80   |
| Medium Risk | 226  |
| High Risk   | 61   |

---

## 💡 Business Use

- Helps banks reduce default risk  
- Supports faster loan decision-making  
- Provides explainable predictions  
- Acts as a decision-support system  

---

## 🖥 Streamlit App

- Input applicant details  
- Predict loan approval  
- View probability score  
- Get risk classification  

---

## ▶️ Run Project (Colab)

(https://colab.research.google.com/drive/1MO_0Zhyxh6OIxwHWk6zud_V5jTdt1lWF?usp=sharing)

---

## ▶️ Run Streamlit

pip install streamlit pyngrok  
streamlit run app.py  

---

## 🧪 Sample Output

{
  "Decision": "APPROVED",
  "Approval_Probability": 0.82,
  "Risk": "Medium Risk"
}

---

## 🛠 Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Random Forest, Logistic Regression  
- SHAP (Explainable AI)  
- Matplotlib, Seaborn  
- Streamlit  

---

## ⭐ Summary

This project demonstrates:
- End-to-end ML pipeline  
- Real-world problem solving  
- Explainable AI  
- Deployment using Streamlit  
