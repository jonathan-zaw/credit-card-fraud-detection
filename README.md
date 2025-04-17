# credit-card-fraud-detection

Detecting credit card fraud with logistic regression and under-sampling.


---

## ***Dataset***
- **Source:** Kaggle (Credit Card Fraud Detection)  
- **Size:** 284,807 rows × 31 columns  
- **Features:** Time, V1–V28 (PCA transformed), Amount, Class  
- **Target Variable:** `Class`  
  - `0` – Legitimate transaction  
  - `1` – Fraudulent transaction  

---

## ***Key Steps***

### **1. Exploratory Data Analysis**
- Checked data types and null values  
- Analyzed class distribution  
- Visualized class imbalance using seaborn count plots  

### **2. Data Imbalance Handling**
- Original dataset is highly imbalanced (only 0.17% fraud)  
- Applied under-sampling to create a balanced subset of 492 fraud and 492 legitimate transactions  

### **3. Feature Engineering**
- Dropped the `Class` column to form the feature matrix `X`  
- Target variable `Y` contains class labels (0 or 1)  

### **4. Model Training**
- **Train-Test Split:** 80% train, 20% test  
- **Model Used:** Logistic Regression  

### **5. Evaluation Metrics**
- Accuracy Score  
- *(Optional for future work: precision, recall, F1-score, ROC-AUC)*  

---

## ***Results***
- Achieved balanced classification accuracy after under-sampling  
- Logistic Regression was able to correctly classify both classes without bias towards the majority class  

