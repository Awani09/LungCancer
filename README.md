# LungCancer
Lung Cancer Prediction Using Machine Learning  
  
Lung cancer is one of the leading causes of death worldwide. Early detection plays a crucial role in improving survival rates. This project uses machine learning techniques to predict the likelihood of lung cancer based on survey responses that capture risk factors such as smoking, alcohol consumption, and respiratory symptoms.  

1. Dataset*  
- The dataset (`survey lung cancer.csv`) contains **309 rows and 16 columns**.  
- Features include demographic details and health conditions:  
  - Categorical Variables: `GENDER` (M/F), `LUNG_CANCER` (YES/NO)  
  - Numerical/Binary Features:  
    - Lifestyle Factors: `SMOKING`, `ALCOHOL CONSUMING`, `PEER_PRESSURE`  
    - Medical Symptoms: `YELLOW_FINGERS`, `ANXIETY`, `WHEEZING`, `COUGHING`, `CHEST PAIN`, etc.  
- Target Variable: `LUNG_CANCER` (Binary classification: "YES" or "NO")  

2. Data Preprocessing  
Before training the models, we perform:  
-Data Cleaning: Checking for missing values and duplicates.  
-Encoding Categorical Variables: Converting `GENDER` and `LUNG_CANCER` into numerical format.  
-Feature Selection: Using techniques like Recursive Feature Elimination (RFE) to select the most important features.  
-Data Splitting: Dividing data into training and test sets (e.g., 80% training, 20% testing).  

3. Machine Learning Models Used  
We experimented with multiple models to find the best-performing one:  
1.Logistic Regression: A simple and interpretable baseline model.  
2.K-Nearest Neighbors (KNN): Measures similarity between data points.  
3.Random Forest Classifier: An ensemble method that combines multiple decision trees.  
4.Gradient Boosting Classifier: An advanced boosting technique that improves predictive accuracy.  
5.XGBoost: A highly optimized gradient boosting library.  
6.Support Vector Machine (SVM): A powerful model for binary classification.  

4. Model Evaluation Metrics  
To assess model performance, we use:  
-Accuracy Score: Percentage of correct predictions.  
-Confusion Matrix: Visualizes correct vs. incorrect predictions.  
-Precision, Recall, F1-score: Measures model effectiveness in handling imbalanced data.  
-ROC Curve & AUC Score: Evaluates classification performance across different thresholds.  

5. Results & Conclusion  
- The best-performing model achieved high accuracy and a strong AUC score, indicating reliable lung cancer predictions.  
- Feature importance analysis showed that `SMOKING`, `AGE`, `WHEEZING`, and `COUGHING` were key indicators of lung cancer risk.  
- This project demonstrates how machine learning can aid in early lung cancer detection, potentially assisting healthcare professionals in risk assessment.  

6. Future Improvements  
-Expanding Dataset: Collecting more diverse and larger datasets for better generalization.  
-Feature Engineering: Extracting new features from patient history or lifestyle habits.  
-Deep Learning: Exploring neural networks for even better predictions.  
-Explain ability: Using SHAP values or LIME to interpret model decisions transparently.  
