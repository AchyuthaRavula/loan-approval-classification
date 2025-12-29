#  Loan Approval Classification using Apache Spark

##  Project Overview
This project builds a **scalable loan approval prediction system** using **Apache Spark (PySpark)** to analyze large-scale financial data and predict whether a loan application will be **approved or rejected**.

The project demonstrates **end-to-end big data analytics**, covering data exploration, feature engineering, and machine learning modeling using Spark MLlib.

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
| Model | Validation Accuracy |
|------|---------------------|
| Logistic Regression | ~78–80% |
| Random Forest | ~83–85% |

 Random Forest improved accuracy by approximately **5%** over Logistic Regression.

---

##  Why This Project Matters
- Processed **45k+ records** using distributed computing
- Built a **production-style ML pipeline** in Spark
- Demonstrated strong understanding of **EDA, feature engineering, and model evaluation**
- Designed notebook and outputs to be **GitHub & recruiter friendly**

---

##  Repository Structure
loan-approval-classification/
│
├── data/ # Dataset placeholder/
├── notebooks/ # PySpark notebook (EDA + ML models)/
├── images/ # Key visualizations used in README/
├── docs/ # Project documentation/
├── README.md # Project overview/
└── LICENSE # MIT License/
---

## ▶️ How to Run
1. Open the notebook in **Databricks** or a Spark-enabled environment
2. Update dataset path if required
3. Run cells sequentially

---
### 🔗 Quick Links
-  [PySpark Notebook](notebooks/BIGDATA_PROJECT.ipynb)
-  [Databricks HTML Output](https://databricks-prod-cloudfront.cloud.databricks.com/...)




