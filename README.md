# **Predict High-Potential HR Service Leads**

## **Project Overview**
This project predicts **high-potential HR service leads** by analyzing **funding and hiring trends** of companies. The dataset includes **synthetic data** that mimics real-world scenarios, and various machine learning models were trained to classify companies as **"hot leads"** using predictive modeling.

---

## **Project Structure**

### 📂 `main.ipynb`
This Jupyter Notebook contains the entire **workflow of the project**, including:
- **Data Preprocessing**
  - Handling missing values  
  - Dealing with infinite values  
  - Encoding categorical variables  
  - Standardizing numerical features  
  - Handling class imbalance using **SMOTE**  
  - Extracting datetime-based features  
- **Feature Engineering**
  - Creating new features from `last_funding_date`
  - Removing irrelevant columns
- **Model Training**
  - Training multiple ML models including Logistic Regression, Random Forest, Gradient Boosting, and XGBoost
- **Model Evaluation**
  - Performance metrics (F1-score, Precision, Recall)
  - Confusion matrix analysis
- **Hyperparameter Tuning**
  - Tuning XGBoost using **RandomizedSearchCV**  

---

### 📂 `DataSets/`
This folder contains:
- **`train.xlsx`** → Raw training dataset  
- **`test.xlsx`** → Raw test dataset  
- **`holdout.xlsx`** → Holdout dataset for final prediction  
- **`Processed_train_data.xlsx`** → Preprocessed training data  
- **`Processed_test_data.xlsx`** → Preprocessed test data  
- **`Processed_holdout_data.xlsx`** → Preprocessed holdout dataset  
- **`submission.xlsx`** → Final submission file  

Each dataset has undergone **data preprocessing** steps to ensure consistency.

---

### 📂 `PKL_files/`
This folder contains essential **saved machine learning artifacts**:
- **`best_xgboost_model.pkl`** → The best-trained XGBoost model after hyperparameter tuning  
- **`scaler.pkl`** → The trained `StandardScaler` object used for feature scaling  
- **`Encoded.pkl`** → The saved encoding mappings for categorical features  

These files ensure **consistent transformation and model inference** across datasets.

---

### 📂 `submission/`
This folder contains:
- **`submission.csv`** → The **final prediction file**, containing:

---

## **HyperParameter Tuning Results**
Before Tuning
![image](https://github.com/user-attachments/assets/ca22e0c7-4294-411b-843e-230d5e9f0664)

After Tuning
![image](https://github.com/user-attachments/assets/9335d805-f017-4442-bac3-6db9bd0b1f37)

---

## **Key Takeaways**
- **Preprocessed data effectively**, ensuring consistency.  
- **Trained multiple ML models**, selecting the best-performing one (**XGBoost**).  
- **Optimized model performance** using hyperparameter tuning.  
- **Standardized workflows** for training, evaluation, and submission.


