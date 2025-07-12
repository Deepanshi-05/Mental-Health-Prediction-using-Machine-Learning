# Mental-Health-Prediction-using-Machine-Learning

This project uses machine learning algorithms to predict levels of **Depression**, **Anxiety**, and **Stress** based on user responses to psychological questionnaires.

---

## 📁 Dataset

The dataset is derived from a mental health survey including:
- 42 psychological questions (DASS-like)
- Demographic details (age, gender, education, etc.)
- Personality measures (TIPI)
- Derived scores and categories for stress, anxiety, and depression

> ⚠️ Invalid or inconsistent responses are filtered using control questions (e.g., `VCL6`, `VCL9`, `VCL12`).

---

## 📊 Project Workflow

1. **Data Cleaning & Preprocessing**
   - Drop incomplete or invalid rows
   - Encode categorical variables
   - Normalize/prepare features

2. **Feature Selection**
   - Retain relevant psychological and demographic columns
   - Extract 3 labels: `CategoryDepr`, `CategoryAnx`, `CategoryStre`

3. **Model Training**
   - Algorithms used:
     - K-Nearest Neighbors (KNN)
     - Naive Bayes (NB)
     - Support Vector Machine (SVM)
     - Random Forest (RF)
     - XGBoost (XGB)

4. **Evaluation**
   - 5-fold Cross-Validation
   - Accuracy used as the primary metric

---

## 🔍 Results Summary

| Model        | Stress Accuracy | Anxiety Accuracy | Depression Accuracy |
|--------------|-----------------|------------------|----------------------|
| KNN          | 49.48%          | 63.07%           | 59.93%               |
| SVC          | 49.48%          | 63.07%           | 59.93%               |
| Naive Bayes  | 93.73%          | 97.21%           | 94.43%               |
| Random Forest| 96.52%          | 94.08%           | 97.56%               |
| XGBoost      | 100.00%         | 100.00%          | 100.00%              |

>  XGBoost outperformed all other models across all three mental health categories.

---

## 🛡️ Ethical Considerations

- This tool is **not a diagnostic tool**, only a prediction based on survey data.
- Should be used for **academic and exploratory purposes only**.

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
