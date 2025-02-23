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


## **Key Takeaways**
- **Preprocessed data effectively**, ensuring consistency.  
- **Trained multiple ML models**, selecting the best-performing one (**XGBoost**).  
- **Optimized model performance** using hyperparameter tuning.  
- **Standardized workflows** for training, evaluation, and submission.

---

 ## **How to Clone and Add Files to This Repository**

### **🔹 Step 1: Clone the Repository**
Open a terminal and run:
```sh
git clone <YOUR_GITHUB_REPO_URL>

Step 2: Navigate to the Repository
sh
Copy
Edit
cd your-repo
🔹 Step 3: Move Project Files into the Repo
Copy your project files into the cloned repo directory.
You can do this manually or use the command:

sh
Copy
Edit
mv /path/to/your/project/* your-repo/
🔹 Step 4: Add Files to Git Tracking
sh
Copy
Edit
git add .
This stages all new and modified files.

🔹 Step 5: Commit the Changes
sh
Copy
Edit
git commit -m "Added machine learning project files"
🔹 Step 6: Push Changes to GitHub
sh
Copy
Edit
git push origin main
