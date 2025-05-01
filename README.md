# 🎓 Student Stress Level Prediction – Data Preprocessing and Classification Project

This project involves analyzing and modeling the **Students Grading Dataset** from Kaggle to understand the patterns behind student stress. It combines two key stages: data preprocessing and machine learning classification using a decision tree model.

---

## 📁 Dataset

- [Students Grading Dataset on Kaggle](https://www.kaggle.com/datasets/mahmoudelhemaly/students-grading-dataset)

The dataset includes academic, behavioral, and lifestyle data such as:
- Exam scores (midterm, final)
- Participation and attendance
- Assignments, quizzes, and project scores
- Sleep and study hours
- Background: gender, department, internet access, parental education
- Target variable: `Stress_Level (1–10)` → transformed into `Stress_Level_Category`

---

## 🧹 Data Preprocessing Steps (Homework 3)

We applied all 5 major preprocessing steps:

### 1. Data Cleaning
- Removed duplicate rows
- Filled missing values using mean imputation for numeric fields
- Standardized string formats (lowercased, trimmed)

### 2. Data Integration
- This step was skipped, as no external datasets were added

### 3. Data Reduction
- Used Attribute Subset Selection to keep only relevant features
- Removed identifiers (e.g., Student_ID, Name, Email)

### 4. Data Transformation
- Applied **Min-Max Normalization** manually to numeric fields
- Scaled all scores and hours to a 0–1 range

### 5. Data Discretization
- Converted `Stress_Level (1–10)` into three labeled categories:
  - Low (0.00–0.33)
  - Medium (0.34–0.66)
  - High (0.67–1.00)
- Created a new target column: `Stress_Level_Category`

**Final preprocessed dataset:** `preprocessed_students_data.csv`

---

## 🧠 Classification Model (Homework 4)

### Model Type: Classification  
We used a supervised classification model to predict which **stress level category** each student belongs to based on their academic and behavioral data.

### Algorithm: Decision Tree Classifier
We chose the **Decision Tree Classifier** because it:
- Works well with structured data
- Handles both categorical and numerical features
- Provides clear decision rules and is easy to visualize

---

## 📊 Results

- **Accuracy:** 100% on the test set
- **Model Evaluation:** Perfect precision, recall, and F1-score for all categories (Low, Medium, High)
- **Key Findings:**
  - `Stress_Level (1–10)` was the most important predictor
  - Other top features: Sleep hours, Final Score, Participation
  - Students with low sleep and low scores had higher stress levels
  - Students with higher performance and sleep were in lower stress categories

---

## 📸 Screenshots to Include

1. Stress Level Distribution Bar Chart
2. Classification Report Output
3. Decision Tree Visualization
4. Feature Importance Chart (Optional)

---

## 📁 Files Included

- `StdGrdClassif.ipynb` – Notebook with all preprocessing + classification code
- `preprocessed_students_data.csv` – Final dataset after preprocessing
- `README.md` – This file
- `report.pdf` – Professional write-up explaining model choice and findings
- Screenshots – PNGs showing key outputs

---

## 🧾 Author

**Erzhigit Kasymbaev**  
Course: Data Mining  
Instructor: Professor Sabina Adhikari

---

