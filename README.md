# Heart Failure Prediction

## Background

In our century, people often prioritize their financial status over their own healthcare, leading to an increase in mental health issues and physical stress. The COVID-19 pandemic has also contributed to heart complications, including muscle damage and impaired heart function (Susan Post, M.D., M.S., 2021). Health centers and medical organizations have accumulated a vast amount of data on heart conditions. With this wealth of information, we can apply machine learning techniques to gain valuable insights.
<br><br>
<div align="center">
  <img src="https://drive.google.com/uc?id=1US_p_u7PYNy2Kfbe3GVweEetK2v3oNC5" alt="Heart Failure Prediction">
  <p><em>The fast growth of heart failure patients from 1970 – 2040: Heart Failure demographics</em></p>
</div>
<br><br>
Prior research has explored heart disease prediction using various methods. In 2011, Ujma Ansari used the Decision Tree model and achieved an accuracy of 99%, inspiring us to use an advanced version, Random Forest (Soni, Jyoti, 2011). Chaitrali S. Dangare, in 2012, used Naive Bayes, Decision Trees, and Neural Networks, adding two more features to the dataset for a total of 15. We aim to refine these approaches by focusing on a dataset with 13 features to avoid overfitting (Dangare, Chaitrali S., and Sulabha S. Apte, 2012).

## Aim

The aim of this project is to predict the likelihood of patients developing heart disease, providing valuable insights to researchers. This knowledge can help in developing better preventive measures and establishing more accurate risk patterns.

## Objectives

1. To develop machine learning models for predicting the likelihood of heart disease, including Logistic Regression, Decision Trees, SVM, and other classification models.
2. To identify high-risk factors contributing to heart issues.
3. To analyze and compare the accuracy of different classification models using the 'heart.csv' dataset.

## Dataset
The dataset used for this project, "Heart Failure Prediction," is sourced from the Kaggle Repository. Can be downloaded manually from This repository.

### Features

The 12 health-related features used in this project are:

- **Age**: Age in years
- **Sex**: (1 = male; 0 = female)
- **ChestPainType**: [TA, ATA, NAP, ASY]
- **RestingBP**: Resting blood pressure (in mm Hg)
- **Cholesterol**: Serum cholesterol in mg/dl
- **FastingBS**: Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
- **RestingECG**: Resting electrocardiographic results
- **MaxHR**: Maximum heart rate achieved
- **ExerciseAngina**: Exercise-induced angina (1 = yes; 0 = no)
- **Oldpeak**: ST depression induced by exercise relative to rest
- **ST_Slope**: The slope of the peak exercise ST segment
- **HeartDisease**: Output column (1 = Heart disease; 0 = Normal)

## Model Training and Evaluation
- **Training**: The models was trained using the `fit` method.
- **Testing**: Tested using the `predict` function, with scaled features for better accuracy.

### Logistic Regression
Logistic Regression is a supervised learning model used for binary classification problems. It is known for its high accuracy and efficiency.


### Decision Trees
Decision Trees are effective for predictive modeling, dividing data into smaller segments.
### Support Vector Machine (SVM)
SVMs are supervised learning algorithms used for classification, effective in high-dimensional spaces.
### Random Forest
Random Forest is a versatile and powerful machine learning technique, often providing excellent results.
### K-Nearest Neighbors (KNN)
KNN is a non-parametric classification method.
### Gaussian Naive Bayes
Gaussian Naive Bayes is a variant that assumes continuous data follows a Gaussian distribution.

## Model Evaluation

To evaluate the models, we used accuracy, precision, recall, F1 score, and cross-validation. These metrics are crucial for assessing the performance of classification models.

### Results

| Model                | Precision (Class 0) | Precision (Class 1) | Recall (Class 0) | Recall (Class 1) | F1 Score (Class 0) | F1 Score (Class 1) | Accuracy | Cross-Val (%) | SD  |
|----------------------|---------------------|---------------------|------------------|------------------|--------------------|--------------------|----------|---------------|-----|
| Logistic Regression  | 0.84                | 0.83                | 0.78             | 0.88             | 0.81               | 0.86               | 84%      | 84            | 0.04|
| Decision Tree        | 0.62                | 0.70                | 0.65             | 0.68             | 0.63               | 0.69               | 75%      | 75            | 0.05|
| SVM                  | 0.86                | 0.82                | 0.76             | 0.90             | 0.81               | 0.86               | 83%      | 83            | 0.04|
| Random Forest        | 0.89                | 0.80                | 0.71             | 0.93             | 0.79               | 0.86               | 83%      | 83            | 0.04|
| K-Nearest Neighbors  | 0.88                | 0.85                | 0.79             | 0.91             | 0.83               | 0.88               | 86%      | 66            | 0.05|
| Gaussian Naive Bayes | 0.88                | 0.79                | 0.70             | 0.92             | 0.78               | 0.85               | 83%      | 83            | 0.04|

The K-Nearest Neighbors model achieved the highest accuracy score of 86%.

## Acknowledgments

Special thanks to Dr. Bashura Sean, Birmingham City University, and all others who contributed to this project.


