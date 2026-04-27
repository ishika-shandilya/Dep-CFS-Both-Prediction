# 🧠 ME/CFS and Depression Prediction — Clinical ML App

Chronic fatigue and depression are frequently misdiagnosed or diagnosed late 
due to overlapping symptoms. This project builds a machine learning system 
that predicts whether a patient has **ME/CFS, Depression, or both** — 
based on clinical and lifestyle inputs.

---

## 💡 Problem Statement

ME/CFS (Myalgic Encephalomyelitis / Chronic Fatigue Syndrome) and Depression 
share several overlapping symptoms — fatigue, sleep disturbances, and low 
social activity — making early diagnosis difficult.

This project answers:
- Can ML models reliably distinguish between ME/CFS, Depression, and comorbid cases?
- Which clinical features are most predictive?
- Can this be made accessible via an interactive app?

---

## 🖥️ Live App

Built and deployed using **Streamlit** — users input patient details and 
receive an instant prediction from their choice of model.

**Input features include:**
- Age, Gender
- Sleep Quality Index & Hours of Sleep
- Brain Fog Level, Fatigue Severity Scale
- Physical Pain Score, Stress Level
- Depression PHQ-9 Score
- PEM (Post-Exertional Malaise) presence and duration
- Work status, Social activity level, Exercise frequency
- Meditation/Mindfulness practice

---

## ⚙️ Models Used

| Model | Description |
|---|---|
| Logistic Regression | Baseline linear classifier |
| Decision Tree | Interpretable rule-based classifier |
| Random Forest | Ensemble model for improved accuracy |

All three models are available for selection within the app — 
allowing direct comparison of predictions.

---

## 🛠️ Tech Stack

- **Python** — Scikit-learn, Pandas, NumPy
- **Streamlit** — Interactive web application
- **Pickle** — Model serialization and deployment

---

## 📂 Repository Structure

├── app.py               # Streamlit application
├── lr1.pkl              # Trained Logistic Regression model
├── pt1.pkl              # Trained Decision Tree model
├── rf1.pkl              # Trained Random Forest model
├── requirements.txt     # Dependencies
└── README.md

---

## 🚀 How to Run Locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

---

## 🔮 Future Improvements

- Add SHAP values for model explainability
- Include XGBoost and compare performance metrics
- Display confusion matrix and ROC curve within the app
- Deploy on Streamlit Cloud for public access
