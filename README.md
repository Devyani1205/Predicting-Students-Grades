Predicting Students Grades
📊 Overview
Machine learning project to predict student performance grades (Fail, Average, Good, Excellent) based on demographic factors and test scores.
Dataset: 1,000 students with 8 features across 4 grade categories
🎯 Features
Demographics: Gender, race/ethnicity, parental education level
Academic Factors: Math scores, reading scores, writing scores, test preparation course completion, lunch type
Engineered Features: Total marks, percentage, grade classification (Fail/Average/Good/Excellent)
🏆 Model Performance
K-Nearest Neighbors - 98.00% ⭐ BEST MODEL
Gradient Boosting - 96.00%
XGBoost - 96.00%
Random Forest - 94.50%
Naive Bayes - 94.00%
Bagging Classifier - 94.00%
Decision Tree - 92.50%
Support Vector Machine - 91.50%
Logistic Regression - 87.50%
AdaBoost - 79.00%
🛠️ Tech Stack
Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn, Joblib


📈 Pipeline
Step 1 - Data Preprocessing: One-hot encoding for categorical features, label encoding for target variable, train-test split with 80-20 ratio and stratification
Step 2 - Feature Engineering: Created total_marks (sum of all scores), percentage calculation, grade categories based on percentage ranges
Step 3 - Model Training: Trained 10 different classification algorithms with optimized hyperparameters
Step 4 - Evaluation: Generated confusion matrices, classification reports, and accuracy comparison visualizations
Step 5 - Model Saving: Serialized all trained models using joblib for future deployment
💡 Key Insights
✅ Students who completed test preparation courses showed significantly better performance across all grades
✅ Female students demonstrated slightly higher average percentages compared to male students
✅ Higher parental education levels strongly correlated with improved student success rates
✅ K-Nearest Neighbors achieved exceptional performance with 98% accuracy on test data
✅ No missing values or duplicates found in the dataset, ensuring high data quality
