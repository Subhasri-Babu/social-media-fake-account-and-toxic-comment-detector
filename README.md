# 🛡️ Social Media Safety System v2.0

> AI-Powered Fake Account Detection & Toxic Comment 
> Classification using 7 Machine Learning Models — 
> Deployed as Live Streamlit Web Application

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![ML](https://img.shields.io/badge/ML-7%20Models-green)
![Accuracy](https://img.shields.io/badge/Accuracy-98%25-brightgreen)
![Streamlit](https://img.shields.io/badge/Streamlit-Live%20App-red)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 🎯 What This Project Does

This project automatically detects two major threats
on social media platforms:

- 🚨 **Fake Accounts** — bots, spam profiles, automated accounts
- 💬 **Toxic Comments** — hate speech, harassment, abuse

The system analyzes 10 behavioral features of any social
media account and classifies it as Real or Fake with
**98% accuracy** using a Stacking Ensemble of 7 ML models.

---

## 🌍 Real World Problem Solved

| Platform   | Daily Fake Accounts Removed | Annual Safety Spend |
|------------|----------------------------|---------------------|
| Instagram  | ~1 Million                 | $1 Billion+         |
| Twitter/X  | ~1 Million bots            | $500 Million+       |
| Facebook   | ~5.4 Billion/quarter       | $5 Billion+         |
| YouTube    | Millions of toxic comments | $2 Billion+         |

> This project replicates the core AI technology used
> by these platforms!

---

## 🤖 7 Machine Learning Models Used

| Model               | Accuracy | Type       |
|---------------------|----------|------------|
| Logistic Regression | 94.17%   | Classical  |
| Decision Tree       | 93.33%   | Classical  |
| Random Forest       | 97.50%   | Ensemble   |
| XGBoost             | 97.00%   | Boosting   |
| LightGBM            | 97.50%   | Boosting   |
| SVM                 | 95.00%   | Kernel     |
| Stacking Ensemble   | 98.00%   | Meta-learn |

**Best Model: Stacking Ensemble (RF + XGBoost + LightGBM)**

---

## ✨ Key Features

- ✅ **7 ML Models** compared and evaluated
- ✅ **BERT NLP** for toxic comment detection
- ✅ **SMOTE** balancing (100 → 900 fake accounts)
- ✅ **5-Fold Cross Validation** for reliable scores
- ✅ **ROC-AUC Curves** professional evaluation
- ✅ **Neural Network** with Early Stopping
- ✅ **Image Augmentation** for profile photos
- ✅ **Feature Importance** analysis (3 models)
- ✅ **Live Streamlit Web App** with 5 tabs
- ✅ **Interactive Plotly Charts** (gauge, radar, bar, pie)
- ✅ **Dark Mode** toggle
- ✅ **Session History** tracking + CSV export
- ✅ **Download Safety Reports** as .txt files
- ✅ **10 ML Concepts** demonstrated in one project

---

## 🌐 Web Application — 5 Tabs

| Tab            | What It Does                              |
|----------------|-------------------------------------------|
| 👤 Fake Detector   | Enter account stats → get AI verdict  |
| 💬 Toxic Comments  | Paste comment → toxicity score        |
| 📊 Analytics       | Interactive model comparison charts   |
| 📋 History Log     | Track all checks + export CSV         |
| ℹ️ About           | Project info + performance summary    |

---

## 🛠️ Technologies Used
```python
# Core
Python 3.10+, NumPy, Pandas

# Machine Learning
Scikit-learn, XGBoost, LightGBM, SMOTE

# Deep Learning & NLP
TensorFlow/Keras, BERT (Hugging Face Transformers)

# Visualization
Matplotlib, Seaborn, Plotly

# Web Application
Streamlit, Plotly

# Deployment
Google Colab, Joblib
```

---

## 📊 Dataset

- **Size:** 1,000 social media accounts
- **Features:** 10 behavioral features
- **Split:** 900 real + 100 fake (imbalanced)
- **After SMOTE:** 900 real + 900 fake (balanced)
- **Also used:** Instagram-pattern dataset (576 accounts)

### 10 Features Analyzed:
```
1. followers        → How many people follow them
2. following        → How many people they follow
3. posts            → Total number of posts
4. bio_length       → Characters in bio
5. has_profile_pic  → Has profile picture?
6. account_age_days → Days since account creation
7. avg_likes        → Average likes per post
8. avg_comments     → Average comments per post
9. verified         → Has verification badge?
10. location_set    → Has location in profile?
```

---

## 🚀 How to Run This Project

### Step 1: Open Google Colab
```
Go to: colab.research.google.com
Create new notebook
```

### Step 2: Install Libraries
```python
!pip install imbalanced-learn xgboost lightgbm
!pip install streamlit plotly transformers torch -q
```

### Step 3: Run All 6 Cells in Order
```
Cell 1 → Install Libraries
Cell 2 → EDA + SMOTE + ML Models + Overfitting
Cell 3 → Neural Network + Early Stopping + Augmentation
Cell 4 → Analysis + Final Summary
Cell A → Install New Libraries (v2.0)
Cell B → 7 Models + BERT + Cross Validation
Cell C → Launch Enhanced Web App v2.0
```

### Step 4: Open Web App
```
Cell C will print a URL like:
https://8502-xxxxx.prod.colab.dev

Click it to open your live web app!
```

---

## 🧪 Sample Test Inputs

### Fake Account Test:
```
followers=10, following=6000, posts=1
bio_length=0, age=5 days, avg_likes=0
→ Result: 100% FAKE 🚨
```

### Real Account Test:
```
followers=850, following=600, posts=45
bio_length=75, age=800 days, avg_likes=120
→ Result: 0% FAKE ✅
```

### Toxic Comment Test:
```
"YOU ARE THE WORST!!! I HATE YOU!!!"
→ Result: 100% TOXIC 🚨
```

### Safe Comment Test:
```
"Great work! Love your content!"
→ Result: 0% TOXIC ✅
```

---

## 📈 Results Summary
```
✅ Best Model Accuracy    : 98.00% (Stacking Ensemble)
✅ Neural Network Accuracy: 97.50%
✅ Early Stopping         : Stopped at epoch 18/100
✅ SMOTE Synthetic Samples: 800 created
✅ Overfitting Gap        : 15% clearly demonstrated
✅ Cross Validation Score : 0.981 ± 0.002
✅ Web App Tests Passed   : 4/4
✅ ML Concepts Used       : 10
```

---

## 🎓 ML Concepts Demonstrated
```
1.  EDA                 → 6 charts, correlation heatmap
2.  Missing Values      → Median & Mode imputation
3.  SMOTE               → Imbalanced data handling
4.  7 ML Models         → Classical + Ensemble + Boosting
5.  Overfitting         → Gap=15% clearly shown
6.  Neural Network      → 3-layer deep learning
7.  Early Stopping      → Optimal epoch detection
8.  Image Augmentation  → 10 profile photo variants
9.  ROC-AUC Curves      → Professional evaluation
10. Web Deployment      → Live Streamlit application
```

---

## 📁 Project Structure
```
social-media-safety-system/
│
├── Cell_1_Install_Libraries.ipynb
├── Cell_2_EDA_SMOTE_Models.ipynb
├── Cell_3_NeuralNetwork_Augmentation.ipynb
├── Cell_4_Analysis_Summary.ipynb
├── Cell_A_Install_New_Libraries.ipynb
├── Cell_B_Advanced_Models.ipynb
├── Cell_C_WebApp.ipynb
├── enhanced_app.py          ← Streamlit web app
├── fake_detector.pkl        ← Saved ML model
├── scaler.pkl               ← Saved scaler
├── requirements.txt         ← All dependencies
└── README.md                ← This file
```

---

## 📋 Requirements
```
pandas
numpy
matplotlib
seaborn
plotly
scikit-learn
xgboost
lightgbm
imbalanced-learn
tensorflow
transformers
torch
streamlit
joblib
```

---

## 🔮 Future Plans

- [ ] Deploy on Streamlit Cloud (permanent URL)
- [ ] Twitter/X API for real account analysis
- [ ] REST API using FastAPI
- [ ] Mobile app (Flutter)
- [ ] Multi-language toxic comment detection
- [ ] SHAP values for explainable AI

---

## 🏆 Project Highlights

> Built a complete AI system that detects fake social
> media accounts and toxic comments with **98% accuracy**
> using 7 machine learning models, BERT NLP, and neural
> networks — deployed as a live interactive web app.
> Solves the same problem that Instagram and Twitter
> spend **billions** solving every year.

---

## 📞 Skills Demonstrated
```
✅ Data Science      → EDA, Cleaning, Analysis
✅ Machine Learning  → 7 different algorithms
✅ Deep Learning     → Neural Networks, BERT
✅ NLP               → Toxic text classification
✅ Imbalanced Data   → SMOTE technique
✅ Model Evaluation  → ROC-AUC, Cross-Validation
✅ Computer Vision   → Image Augmentation
✅ Web Development   → Streamlit Dashboard
✅ Data Visualization→ Matplotlib + Plotly
✅ Deployment        → Live public URL
```

---

## ⭐ If you found this helpful, please star this repo!

---

*Built with Python & Machine Learning*
*Google Colab | Streamlit | Scikit-learn | XGBoost | BERT*
```

---

## 🏷️ GitHub Topics/Tags to Add:
```
machine-learning
python
streamlit
fake-account-detection
toxic-comment-detection
xgboost
lightgbm
bert-nlp
deep-learning
smote
data-science
social-media
nlp
random-forest
plotly

8. Paste the full README above
9. Add topics/tags
10. Click Save ✅
