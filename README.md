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
pip install pandas numpy scikit-learn xgboost matplotlib seaborn joblib
```

### Installation Steps
1. Clone the repository
```bash
git clone https://github.com/yourusername/predicting-students-grades.git
cd predicting-students-grades
```

2. Install required packages
```bash
pip install -r requirements.txt
```

3. Run the Jupyter notebook
```bash
jupyter notebook student_performance_analysis.ipynb
```

### Usage Example
```python
import joblib

# Load the best model
model = joblib.load('saved_models/K-Nearest_Neighbors.joblib')

# Make predictions
predictions = model.predict(new_data)
```

## 📈 Machine Learning Pipeline

### 1. Data Preprocessing
- Checked for missing values (none found)
- Verified no duplicate records
- Applied one-hot encoding for categorical features
- Applied label encoding for target variable
- Split data: 80% training, 20% testing with stratification

### 2. Feature Engineering
- Created `total_marks` feature (sum of math, reading, writing scores)
- Calculated `percentage` from total marks
- Classified grades into 4 categories based on percentage

### 3. Model Training
- Trained 10 different classification algorithms
- Applied optimized hyperparameters for each model
- Used stratified sampling to maintain class distribution

### 4. Model Evaluation
- Generated confusion matrices for all models
- Created classification reports with precision, recall, F1-score
- Visualized accuracy comparison across models
- Analyzed performance metrics for each grade category

### 5. Model Deployment
- Saved all trained models using joblib
- Created model files in `saved_models/` directory
- Models ready for production deployment

## 💡 Key Insights

### Performance Factors
- ✅ Test preparation course completion significantly improves student grades
- ✅ Female students show slightly higher average percentages
- ✅ Higher parental education strongly correlates with better student performance
- ✅ Standard lunch program students outperform free/reduced lunch students

### Data Quality
- ✅ Clean dataset with no missing values
- ✅ No duplicate records found
- ✅ Balanced distribution across demographic categories
- ✅ Normal score distributions for all subjects

### Model Results
- ✅ K-Nearest Neighbors achieved exceptional 98% accuracy
- ✅ Ensemble methods (Gradient Boosting, XGBoost) performed consistently well
- ✅ All models except AdaBoost achieved >87% accuracy
- ✅ High precision and recall across all grade categories

## 📂 Project Structure
```
predicting-students-grades/
│
├── data/
│   └── StudentsPerformance.csv
│
├── saved_models/
│   ├── K-Nearest_Neighbors.joblib
│   ├── Gradient_Boosting.joblib
│   ├── XGBoost.joblib
│   ├── Random_Forest.joblib
│   ├── Naive_Bayes.joblib
│   ├── Bagging_Classifier.joblib
│   ├── Decision_Tree.joblib
│   ├── Support_Vector_Machine.joblib
│   ├── Logistic_Regression.joblib
│   └── AdaBoost.joblib
│
├── student_performance_analysis.ipynb
├── requirements.txt
├── README.md
└── .gitignore
```

## 📊 Visualizations Included

### Exploratory Data Analysis
- Count plots for categorical features
- Distribution histograms for numerical scores
- Box plots for outlier detection
- Scatter plots for feature relationships
- Gender vs grade performance comparison
- Test preparation impact analysis

### Model Evaluation
- Confusion matrices for all 10 models
- Accuracy comparison bar chart
- Classification report metrics
- Performance visualization by grade category

## 🔮 Future Enhancements

### Model Improvements
- Implement GridSearchCV for hyperparameter tuning
- Perform cross-validation for robust evaluation
- Experiment with ensemble stacking techniques
- Try deep learning models (Neural Networks)

### Feature Engineering
- Create interaction features between demographics
- Analyze feature importance using SHAP values
- Include additional external factors (attendance, study hours)

### Deployment
- Build REST API using Flask/FastAPI
- Create interactive web app with Streamlit
- Deploy on cloud platforms (AWS, Heroku, Azure)
- Implement real-time prediction system

### Analysis
- Conduct deeper statistical analysis
- Identify at-risk students early
- Provide personalized recommendations
- Generate automated performance reports

## 📝 Model Details

### K-Nearest Neighbors (Best Model)
- **Accuracy**: 98.00%
- **Parameters**: n_neighbors=10
- **Strengths**: Excellent performance across all grade categories
- **Metrics**:
  - Average: Precision 0.97, Recall 0.97
  - Excellent: Precision 1.00, Recall 1.00
  - Fail: Precision 1.00, Recall 0.95
  - Good: Precision 0.97, Recall 0.99

## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📧 Contact
For questions or feedback, please open an issue in the repository.

## 🙏 Acknowledgments
- **Dataset Source**: Kaggle - Students Performance in Exams
- **Inspiration**: Educational data mining and predictive analytics
- **Libraries**: Scikit-learn, XGBoost, and pandas development teams

---

**⭐ Star this repository if you found it helpful!**

**📌 Project Status**: Complete and ready for deployment

**🎯 Key Achievement**: 98% prediction accuracy with K-Nearest Neighbors
