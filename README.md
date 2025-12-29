#  Loan Approval Classification using Apache Spark

## Project Overview

This project builds a **scalable loan approval classification system** using **Apache Spark (PySpark)** to analyze large-scale financial data and predict whether a loan application will be **approved or rejected**.

The solution demonstrates an **end-to-end big data analytics pipeline**, including:
- Exploratory Data Analysis (EDA)
- Feature engineering and encoding
- Machine learning model development using **Spark MLlib**

Two classification models were implemented and evaluated:
- **Logistic Regression**
- **Random Forest**, achieving up to **92% accuracy** on validation data

This project highlights the application of **big data processing, distributed machine learning, and model evaluation** for real-world financial decision-making.

---

##  Dataset
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/taweilo/loan-approval-classification-data)
- **Records:** **45,000+ loan applications**  
- **Features:** **14 variables** (demographic, financial, and loan-related)  
- **Target Variable:** `loan_status` (Approved / Rejected)

---

##  Tech Stack
- **Big Data Framework:** Apache Spark (PySpark)
- **Machine Learning:** Spark MLlib  
  - Logistic Regression  
  - Random Forest Classifier
- **Data Processing:** PySpark DataFrames
- **Visualization:** Matplotlib, Seaborn
- **Environment:** Databricks / Jupyter Notebook

---

##  Exploratory Data Analysis (EDA)
Key analyses performed:
- Distribution analysis for numerical features (age, income, loan amount, credit score)
- Categorical feature analysis (education, gender, loan intent, home ownership)
- Outlier detection using box plots
- Missing value analysis (**0 missing values across all features**)

 **Key Insights**
- Majority of applicants fall between **20–40 years of age**
- Higher approval likelihood observed for applicants with **higher credit scores**
- Dataset required **no imputation**, enabling direct model training

---

##  Feature Engineering
- Encoded categorical variables using indexing and ordinal techniques
- Assembled features using `VectorAssembler`
- Standardized numerical features using `StandardScaler`
- Prepared clean feature vectors for ML pipelines

---

##  Model Development
### Models Implemented
1. **Logistic Regression**
   - Interpretable baseline model
2. **Random Forest Classifier**
   - Captures non-linear relationships

### Data Split
- **Training:** 80%
- **Validation:** 20%
- **Seed:** Fixed for reproducibility

---

##  Model Performance
We trained and evaluated two machine learning models using **Apache Spark MLlib** on a dataset of **45,000+ loan applications**.

| Model | Accuracy |
|------|----------|
| Logistic Regression | **0.89** |
| Random Forest Classifier | **0.92**  |

 **Best Performing Model:** Random Forest  
 **Improvement over baseline:** +3% accuracy  
 **Evaluation Metric:** Accuracy (Spark MulticlassClassificationEvaluator)

The Random Forest model outperformed Logistic Regression by effectively capturing non-linear relationships among borrower demographics, credit history, and loan characteristics.


---

##  Why This Project Matters
- Processed **45k+ records** using distributed computing
- Built a **production-style ML pipeline** in Spark
- Demonstrated strong understanding of **EDA, feature engineering, and model evaluation**
- Designed notebook and outputs to be **GitHub & recruiter friendly**

---

##  How to Run
1. Open the notebook in **Databricks** or a Spark-enabled environment 
2. Update dataset path if required
3. Run cells sequentially




