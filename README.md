# 🧠 Healthcare Data Analysis and Predictive Modeling

## 📌 Overview
This project demonstrates a complete data science workflow applied to a synthetic healthcare dataset from [Kaggle](https://www.kaggle.com/datasets/prasad22/healthcare-dataset). It includes feature engineering, exploratory data analysis (EDA), machine learning modeling, and an interactive dashboard built with Tableau.

The main objective is to predict **Test Results** ("Normal", "Abnormal", "Inconclusive") based on patient demographics, medical conditions, and admission details.





## 📅 Project Timeline
- **Started:** February 2025  
- **Completed:** March 2025  
- **Uploaded to GitHub:** November 2025





## 📁 Project Structure

```
DataScienceFinalProject/
│
├── data/
│   └── healthcare_dataset.csv
│
├── notebooks/
│   ├── Final Task (Analysis).ipynb
│   └── Final Task (ML).ipynb
│
├── models/
│   ├── healthcare(RandomForest Without FS).pkl
│   └── healthcare(RandomForest With FS).pkl
│
├── reports/
│   ├── Final Task (Python).pptx
│   └── report.pdf
│
├── tableau/
│   └── Data Science Final Project.twb
│
├── README.md
├── requirements.txt
└── tableau_dashboard_link.txt
```



## 🧪 Dataset Description
The dataset contains 10,000 synthetic patient records with the following attributes:
- **Demographics:** Name, Age, Gender, Blood Type  
- **Medical Info:** Medical Condition, Medication, Test Results  
- **Admission Details:** Admission Type, Date of Admission, Discharge Date, Doctor, Hospital, Room Number  
- **Financial Info:** Insurance Provider, Billing Amount





### 📂 Dataset Source
- Original dataset from Kaggle: [Healthcare Dataset](https://www.kaggle.com/datasets/prasad22/healthcare-dataset)
- A local copy (`healthcare_dataset.csv`) is included in the `data/` folder for reproducibility.





## 🧹 Data Preprocessing
The following preprocessing steps were applied:
- Calculated **Length of Stay (LOS)** from admission and discharge dates
- Encoded categorical features (e.g., Gender, Blood Type, Medical Condition)
- Scaled numerical features using `StandardScaler` and `MinMaxScaler`
- Split the dataset into training and testing sets

> No missing value cleaning was required for this dataset.





## 📈 Exploratory Data Analysis (EDA)
Performed using `pandas`, `matplotlib`, and `seaborn`:
- Age distribution
- Gender counts
- Blood type distribution
- Most common medical conditions
- LOS statistics
- Insurance and billing analysis
- Admission type breakdown
- Medication and test result frequencies





## 🤖 Machine Learning Modeling

### Models Trained (Before Feature Selection):
1. Logistic Regression  
2. Decision Tree  
3. Random Forest  
4. Support Vector Machine (SVM)  
5. K-Nearest Neighbors (KNN)

### Feature Selection Techniques:
Each model was retrained using features selected by a dedicated algorithm:
- Feature Selection for Logistic Regression  
- Feature Selection for Decision Tree  
- Feature Selection for Random Forest  
- Feature Selection for SVM

### Saved Models:
- `healthcare(RandomForest Without FS).pkl`: Best-performing model before feature selection  
- `healthcare(RandomForest With FS).pkl`: Best-performing model after feature selection

### Evaluation Metrics:
- Accuracy  
- Confusion Matrix  
- ROC Curve  
- Precision, Recall, F1-score





## 📊 Tableau Dashboard
An interactive dashboard was created using **Tableau Public** to visualize:
- Age and gender distributions  
- Medical condition frequencies  
- LOS and billing insights  
- Medication and test result breakdowns  
- Predictive model summaries

🔗 [View Dashboard on Tableau Public](https://public.tableau.com/views/DataScienceFinalProject_17386220148420/Dashboard1)





## ⚙️ Installation

Install the required libraries:
```bash
pip install -r requirements.txt
```

Run the notebooks:

``` 
jupyter notebook "Final Task (Analysis).ipynb"
jupyter notebook "Final Task (ML).ipynb"

```







## 📦 Requirements

The project uses the following Python libraries:
- pandas  
- numpy  
- seaborn  
- matplotlib  
- scikit-learn

These are listed in the `requirements.txt` file





## 👤 Author

**Eng. Hala Shehada**  
Course: Data Science Fundamentals  
Instructor: Eng. Dr. Ali Atia  
Institution: Darrebni Company