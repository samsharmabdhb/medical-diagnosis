# medical-diagnosis
AI-ML projects 
# 🩺 Disease Prediction Using Machine Learning

This project is a symptom-based disease prediction system using an ensemble of machine learning classifiers. Given a set of symptoms, it predicts the most likely disease using Random Forest, Naive Bayes, and SVM, combined through majority voting or soft voting.

---

## 📌 Features

- Predict disease from symptoms using:
  - Random Forest
  - Naive Bayes
  - Support Vector Machine (SVM)
- Data balancing using Random Oversampling
- Ensemble voting for robust prediction
- Confusion matrix and performance visualization
- Scalable for web/app deployment
- Input symptom-based prediction interface

---

## 🧠 Models Used

- `RandomForestClassifier`
- `GaussianNB`
- `SVC (with probability=True for soft voting)`

---

## 📊 Dataset

- The dataset is a cleaned CSV file containing symptoms as features and diseases as the target.
- Each row corresponds to a possible combination of symptoms and associated disease.

---

## ⚙️ Requirements

```bash
pip install -r requirements.txt

git clone https://github.com/yourusername/disease-prediction-ml

predict_disease("Itching,Skin Rash,Nodal Skin Eruptions")

Voting System
The system predicts using all three models and selects the majority vote (mode) as the final prediction. Alternatively, you can use soft voting based on predicted probabilities.

Evaluation
Accuracy, confusion matrices, and classification reports are used to evaluate model performance.

Ensemble models tested on resampled and test-split data aim to reach 80%+ accuracy.

Future Enhancements
Web interface using Flask or Streamlit

Fuzzy matching for symptom entry

Deep learning-based classifier

Integration with real-time symptom APIs
