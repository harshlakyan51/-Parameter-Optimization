# -Parameter-Optimization
# 📊 SVM Optimization on UCI HAR Dataset

This project applies Support Vector Machine (SVM) classification on the **Human Activity Recognition Using Smartphones (HAR)** dataset from the UCI Machine Learning Repository. The SVM model is optimized over different hyperparameters across 10 randomly sampled datasets, and the convergence graph is plotted for the best-performing model.

---

## 📁 Dataset Description

**Dataset:** [UCI HAR Dataset](https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones)  
**Samples:** 10,299  
**Classes:** 6 (e.g., walking, standing, lying, etc.)  
**Features:** 561 numeric features (accelerometer and gyroscope signals)

---

## 🎯 Objective

- Use **NuSVC** (a variant of SVM) to classify human activities.
- Perform **hyperparameter optimization** (`kernel`, `nu`, `gamma`) using GridSearchCV.
- Run experiments on **10 different samples**, each of size 5000.
- Record the **best accuracy and parameters** for each sample.
- Plot a **convergence graph** of accuracy over iterations for the best-performing sample.

---

## 🧪 Tools & Libraries

- Python 3.x
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Requests
- Zipfile

---


---

## 🧠 How It Works

1. **Dataset Download & Load:** HAR dataset is downloaded and combined from train/test splits.
2. **Sampling:** For each of the 10 iterations, a random sample of 5000 records is drawn.
3. **Training & Tuning:** Train SVM using a grid search over kernel types and `nu` values.
4. **Evaluation:** Accuracy is recorded on a held-out test set (30%).
5. **Plotting:** The convergence graph for the best accuracy sample is generated.

---

## 📊 Table 1:  Output Format

![image](https://github.com/user-attachments/assets/8516f9e8-bc4a-45d6-9c8a-08327753f87a)

## 📈  Convergence Graph

The following plot shows how accuracy improves across iterations (simulated for visualization):
![image](https://github.com/user-attachments/assets/d4a9cc88-39d8-4f69-9d87-8eb282e73a36)


