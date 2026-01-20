# Sampling Techniques on Credit Card Fraud Dataset

## 📌 Objective

The objective of this assignment is to study the impact of **different sampling techniques** on the performance of **various machine learning models** using an imbalanced credit card fraud dataset.

---

## 📂 Dataset

* **Name:** Creditcard_data.csv
* **Target Variable:** `Class`

  * `0` → Non-Fraud
  * `1` → Fraud

The dataset is highly imbalanced, so balancing techniques are required before model training.

---

## ⚙️ Steps Performed

1. Load the dataset from GitHub
2. Separate features and target variable
3. Convert the imbalanced dataset into balanced datasets using different sampling techniques
4. Create five samples
5. Apply five different machine learning models on each sampling technique
6. Compare accuracy scores
7. Identify the best sampling technique for each model

---

## 🔁 Sampling Techniques Used

| Sampling Name | Technique                                          |
| ------------- | -------------------------------------------------- |
| Sampling1     | Random Under Sampling                              |
| Sampling2     | Random Over Sampling                               |
| Sampling3     | SMOTE (Synthetic Minority Over-sampling Technique) |
| Sampling4     | Tomek Links                                        |
| Sampling5     | SMOTE + Tomek Links                                |

---

## 🤖 Machine Learning Models Used

| Model | Algorithm                 |
| ----- | ------------------------- |
| M1    | Logistic Regression       |
| M2    | Decision Tree Classifier  |
| M3    | Random Forest Classifier  |
| M4    | K-Nearest Neighbors (KNN) |
| M5    | Naive Bayes               |

---

## 📊 Accuracy Results (%)

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
| ----- | --------- | --------- | --------- | --------- | --------- |
| M1    | 50.10     | 52.24     | 63.18     | 69.23     | 70.12     |
| M2    | 59.25     | 65.27     | 68.72     | 28.36     | 30.25     |
| M3    | 90.45     | 72.41     | 32.17     | 42.58     | 41.85     |
| M4    | 78.25     | 56.24     | 47.23     | 33.44     | 40.12     |
| M5    | 81.25     | 12.85     | 57.36     | 32.25     | 52.74     |

---

## 🏆 Best Sampling Technique for Each Model

| Model | Best Sampling | Accuracy |
| ----- | ------------- | -------- |
| M1    | Sampling5     | 70.12%   |
| M2    | Sampling3     | 68.72%   |
| M3    | Sampling1     | 90.45%   |
| M4    | Sampling1     | 78.25%   |
| M5    | Sampling1     | 81.25%   |

---

## 📌 Observations

* Random Under Sampling performed best for most models.
* Random Forest achieved the highest accuracy among all models.
* Sampling technique selection has a significant impact on model performance.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Imbalanced-learn


## ✅ Conclusion

This experiment demonstrates that balancing techniques are crucial for handling imbalanced datasets. Proper selection of sampling methods can significantly improve classification accuracy, especially for fraud detection problems.
