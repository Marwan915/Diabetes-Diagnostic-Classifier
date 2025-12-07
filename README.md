# 🩺 Diabetes Diagnosis using Decision Tree

## 📌 Project Overview
This project focuses on developing a machine learning classification model to diagnose diabetes in patients based on various clinical and laboratory features. Using a **Decision Tree Classifier**, the model categorizes patients into three distinct classes: **Diabetic**, **Non-Diabetic**, and **Predict-Diabetic**.

## 🚀 Key Results
- **Model Accuracy:** Achieved an impressive **99.33%** accuracy on the test set.
- **Robustness:** Successfully avoided overfitting by tuning the `max_depth` hyperparameter.
- **Interpretability:** The model logic can be visualized as a tree structure, making clinical decisions transparent.

## 📊 Dataset & Features
The model was trained on a dataset of 1,000 patient records containing the following features:
- **Demographics:** Age, Gender.
- **Clinical Indicators:** BMI (Body Mass Index).
- **Lab Tests:** Urea, Creatinine (Cr), HbA1c, Cholesterol (Chol), Triglycerides (TG), HDL, LDL, VLDL.
- **Target Class:**
    - `N`: Non-Diabetic
    - `P`: Predict-Diabetic
    - `Y`: Diabetic

## 🛠️ Methodology

### 1. Data Preprocessing
- **Cleaning:** Removed unnecessary columns (`ID`, `No_Pation`) and handled whitespace in column names.
- **Encoding:** - Converted `Gender` to numeric (M=1, F=0).
    - Mapped target classes (`N`, `P`, `Y`) to numeric values (`0`, `1`, `2`).
- **Data Integrity:** Removed rows with missing values to ensure quality training.

### 2. Model Development
- **Splitting:** The dataset was split into Training, Validation, and Testing sets to ensure unbiased evaluation.
- **Algorithm:** Used `DecisionTreeClassifier` from Scikit-Learn.
- **Hyperparameter Tuning:** Experimented with different `max_depth` values (ranging from 2 to 15) to find the optimal tree depth that maximizes accuracy on validation data without overfitting.
    - *Optimal Depth Found:* **4**

### 3. Evaluation
- The model was evaluated using:
    - **Accuracy Score**
    - **Confusion Matrix:** To visualize misclassifications.
    - **Tree Visualization:** Generated a graphical representation of the decision tree logic.

## 💻 Technologies Used
- **Python**
- **Pandas:** Data manipulation and cleaning.
- **Scikit-Learn:** Model building, splitting, and metrics.
- **Matplotlib & Pyplot:** Visualizing the decision tree and confusion matrix.

---
*Developed by Marwan Ali*
