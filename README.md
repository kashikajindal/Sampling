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
| M1    | 66.67     | 91.70     | 90.39     | 98.70     | 92.17     |
| M2    | 66.67     | 98.47     | 98.25     | 97.39     | 98.43     |
| M3    | 50.00     | 99.78     | 99.34     | 98.70     | 99.55     |
| M4    | 16.67     | 98.47     | 84.72     | 98.70     | 85.23     |
| M5    | 50.00     | 78.17     | 84.50     | 95.22     | 89.26     |

---

## 🏆 Best Sampling Technique for Each Model

| Model | Best Sampling | Accuracy |
| ----- | ------------- | -------- |
| M1    | Sampling4     | 98.70%   |
| M2    | Sampling2     | 98.47%   |
| M3    | Sampling2     | 99.78%   |
| M4    | Sampling4     | 98.70%   |
| M5    | Sampling4     | 95.22%   |

---

## 📌 Observations

* Sampling4 (Tomek Links) produced the best results for most models.
* Sampling2 (Random Over Sampling) worked best for Decision Tree and Random Forest models.
* Random Forest (M3) achieved the highest overall accuracy (99.78%).
* Sampling techniques significantly influence model performance on imbalanced datasets.
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
