# Predicting Students Grades

## 📊 Project Overview
Machine learning project to predict student performance grades (Fail, Average, Good, Excellent) based on demographic factors and test scores.

- **Dataset Size**: 1,000 students
- **Features**: 8 input features
- **Target Classes**: 4 grade categories
- **Best Accuracy**: 98.00%

## 🎯 Features Description

### Demographic Features
- Gender (male/female)
- Race/ethnicity (Group A-E)
- Parental level of education

### Academic Features
- Math score (0-100)
- Reading score (0-100)
- Writing score (0-100)
- Test preparation course (completed/none)
- Lunch type (standard/free-reduced)

### Engineered Features
- Total marks (sum of all scores)
- Percentage (total/300 × 100)
- Grade classification:
  - Fail: 0-50%
  - Average: 51-65%
  - Good: 66-80%
  - Excellent: 81-100%

## 🏆 Model Performance

### Top 3 Models
1. **K-Nearest Neighbors** - 98.00% ⭐ BEST MODEL
2. **Gradient Boosting** - 96.00%
3. **XGBoost** - 96.00%

### Other Models
- Random Forest - 94.50%
- Naive Bayes - 94.00%
- Bagging Classifier - 94.00%
- Decision Tree - 92.50%
- Support Vector Machine - 91.50%
- Logistic Regression - 87.50%
- AdaBoost - 79.00%

## 🛠️ Technologies Used

### Programming Language
- Python 3.x

### Libraries
- **Data Manipulation**: Pandas, NumPy
- **Machine Learning**: Scikit-learn, XGBoost
- **Visualization**: Matplotlib, Seaborn
- **Model Persistence**: Joblib

## 🚀 Getting Started

### Prerequisites
```bash
