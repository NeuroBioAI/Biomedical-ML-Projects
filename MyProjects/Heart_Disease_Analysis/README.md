# ❤️ Heart Disease Analysis

## Project Objective
The goal of this project is to predict whether a patient has heart disease using various medical features and machine learning algorithms. Accurate prediction can help in early diagnosis and timely treatment, potentially saving lives.

Two popular machine learning models were implemented and compared:
- K-Nearest Neighbors (KNN)
- Decision Tree Classifier

The dataset includes demographic, clinical, and diagnostic features, and model performance is evaluated using Accuracy, Precision, Recall, and F1-score.

## Data Source
The dataset and feature descriptions were obtained from [Heart Disease Dataset Source](<link-to-website>).

## Features
1. Age: Age of the patient [years]
2. Sex: Sex of the patient (M: Male, F: Female)
3. ChestPainType: Chest pain type (TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptotic)
4. RestingBP: Resting blood pressure [mmHg]
5. Cholesterol: Serum cholesterol [mg/dl]
6. FastingBS: Fasting blood sugar (1: FastingBS > 120 mg/dl, 0: otherwise)
7. RestingECG: Resting electrocardiogram results (Normal, ST: ST-T wave abnormality)
8. MaxHR: Maximum heart rate achieved [60-202]
9. ExerciseAngina: Exercise-induced angina (Y: Yes, N: No)
10. Oldpeak: Depression measured by exercise test [numeric]
11. ST_Slope: Slope of the peak exercise ST segment (Up, Flat, Down)
12. HeartDisease: Target class (1: Heart disease, 0: Normal)

## Project Structure
- heart_disease_analysis.ipynb : Main Jupyter Notebook
- heart_disease.csv : Dataset file
- README.md : Project documentation
- requirements.txt : Python packages (optional)

## Exploratory Data Analysis (EDA)
A thorough exploratory data analysis was conducted to check for missing values, visualize feature distributions, and explore correlations among features. Insights gained from EDA guided feature selection and modeling.

## Methodology
- Data preprocessing: encoding categorical features and scaling numeric values
- Train/test split
- Training KNN and Decision Tree classifiers
- Evaluating models using Accuracy, Precision, Recall, F1-score, and Confusion Matrices

## Results

### K-Nearest Neighbors (KNN)
- Accuracy: 0.73
- F1-score: Class 0 = 0.73, Class 1 = 0.78

### Decision Tree Classifier
- Accuracy: 0.83
- F1-score: Class 0 = 0.81, Class 1 = 0.85

### Model Comparison
Decision Tree outperforms KNN in all metrics, providing higher accuracy and F1-scores for both classes.

## Technologies
- Python 3.x
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## Author
Monireh Arina
Biomedical Engineer | In Silico Drug Design Enthusiast | AI in Medicine Explorer

