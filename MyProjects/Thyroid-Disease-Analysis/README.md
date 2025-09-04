# 🦋 Thyroid Disease Analysis

## Project Goal
This dataset is about thyroid diseases and cancer. Medical information of 383 patients was collected with 17 features including age, gender, smoking, Hx smoking, Hx Radiotherapy, Thyroid Function, Physical Examination, Adenopathy, Pathology, Focality, Risk, T (Tumor classification), N (Nodal classification), M (Metastasis classification), Stage, Response, and Recurred.

The goal of this project is to train two models:
1. To predict whether the disease recurred after treatment (Recurred).
2. To predict the patient's response to treatment (Response).

## Model Training
After exploratory data analysis (EDA), we aim to train two models for the following tasks:

- Predict if the disease will recur after treatment (Recurred)
- Predict the patient's response to treatment (Response)

We employ Decision Tree classifiers for both tasks.

## Features Introduction
- **Age:** The age of the patient at the time of diagnosis or treatment.
- **Gender:** The gender of the patient (male or female).
- **Smoking:** Whether the patient is a smoker or not.
- **Hx Smoking:** Smoking history of the patient.
- **Hx Radiotherapy:** History of radiotherapy treatment for any condition.
- **Thyroid Function:** The status of thyroid function.
- **Physical Examination:** Findings from a physical examination of the patient.
- **Adenopathy:** Presence or absence of enlarged lymph nodes.
- **Pathology:** Specific types of thyroid cancer.
- **Focality:** Whether the cancer is unifocal or multifocal.
- **Risk:** The risk category of the cancer.
- **T:** Tumor classification.
- **N:** Nodal classification.
- **M:** Metastasis classification.
- **Stage:** Overall stage of the cancer.
- **Response:** Response to treatment.
- **Recurred:** Indicates whether the cancer has recurred.

## Result

### Model 1: Predicting Disease Recurrence (Recurred)
- **Accuracy:** 0.96  
- **Precision, Recall, F1-Score:**
  - Class 0 (No recurrence): Precision 0.98, Recall 0.96, F1-Score 0.97  
  - Class 1 (Recurrence): Precision 0.91, Recall 0.95, F1-Score 0.93  
- **Macro Average:** Precision 0.95, Recall 0.96, F1-Score 0.95  
- **Weighted Average:** Precision 0.96, Recall 0.96, F1-Score 0.96  

These results indicate that the Decision Tree classifier performs very well in predicting disease recurrence.

### Model 2: Predicting Patient Response to Treatment (Response)
- **Accuracy:** 0.70  
- **Precision, Recall, F1-Score:**
  - Class 0: Precision 0.40, Recall 0.40, F1-Score 0.40 (n=5)  
  - Class 1: Precision 0.76, Recall 0.81, F1-Score 0.78 (n=42)  
  - Class 2: Precision 0.20, Recall 0.17, F1-Score 0.18 (n=12)  
  - Class 3: Precision 0.94, Recall 0.89, F1-Score 0.91 (n=18)  
- **Macro Average:** Precision 0.57, Recall 0.57, F1-Score 0.57  
- **Weighted Average:** Precision 0.69, Recall 0.70, F1-Score 0.69  

These results indicate that the Decision Tree classifier shows good performance for some classes (especially class 3), but lower performance for others, highlighting areas for potential improvement in predicting treatment response.

## File Structure
- `thyroid_analysis.ipynb` : Main Jupyter Notebook with all analysis and modeling  
- `Thyroid_Diff.csv` : Dataset used in the project  
- `README.md` : Project documentation  
- `requirements.txt` : List of required Python packages (optional)

## How to Run
1. Clone this repository:
   ```bash
   git clone <your-repo-link>
   ```
2. Install required packages:
   ```bash
   pip install scikit-learn pandas matplotlib seaborn
   ```
3. Open `thyroid_analysis.ipynb` in Jupyter Notebook and run the cells.

