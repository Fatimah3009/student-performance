# student-performance


# 📘 Student Performance Prediction

## 📌 Project Overview

This project predicts students’ **exam scores** based on various factors such as **study hours, attendance, previous scores, and tutoring sessions**.
It uses **Linear Regression** and **Polynomial Regression**, with comparisons of performance metrics.

---

## 📂 Dataset

* Source: [Kaggle – Student Performance Factors](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors?resource=download)
* Key Features:

  * `Hours_Studied` → Study hours per day
  * `Attendance` → Percentage of classes attended
  * `Previous_Scores` → Average of past exam scores
  * `Tutoring_Sessions` → Number of tutoring sessions attended
  * `Exam_Score` → Final target variable (exam score)

---

## 🛠️ Tools & Libraries

* Python
* Pandas, NumPy
* Matplotlib, Seaborn (visualization)
* Scikit-learn (machine learning models & metrics)

---

## 📊 Model Training

1. **Linear Regression** (using study hours only) → Low R² (\~23%)
2. **Polynomial Regression** (study hours only) → Still low (\~23%)
3. **Multiple Linear Regression** (Hours\_Studied, Attendance, Previous\_Scores, Tutoring) → **R² \~64%**

---

## 📈 Results

* **Best Model**: Multiple Linear Regression
* **Performance**:

  * MAE ≈ 1.27
  * MSE ≈ 5.06
  * R² ≈ 0.64 (\~64% accuracy)
* Key Insight: **Attendance** had the strongest impact on exam scores, more than study hours.

---

## 📷 Visualizations

* Correlation heatmap of features
* Scatter plot: Hours Studied vs Exam Score
* Linear vs Polynomial regression fits

---

## 🚀 How to Run

1. Clone this repo

   ```bash
   git clone https://github.com/your-username/student-performance.git
   cd student-performance
   ```
2. Open the Jupyter/Colab notebook:

   ```bash
   Student_Performance_Prediction.ipynb
   ```
3. Run all cells to train models and see results.

---

## 📌 Future Improvements

* Try **Random Forest / Gradient Boosting** for better accuracy
* Add more student-related features (e.g., stress level, family support)
* Build a **Streamlit web app** for interactive predictions

---

