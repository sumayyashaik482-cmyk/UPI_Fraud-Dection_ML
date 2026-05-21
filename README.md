# UPI_Fraud-Dection_ML
UPI fraud detection in Python Using Machine Learning

## 📌 Project Summary
With the rapid increase in **UPI-based digital transactions**, fraud detection has become a critical requirement in the financial sector.

This project presents a **Machine Learning-based Fraud Detection System** that identifies fraudulent UPI transactions using **Random Forest Classifier** and handles class imbalance using **SMOTE (Synthetic Minority Oversampling Technique)**.

The system is designed to simulate a **real-world fintech fraud detection pipeline**.

## 🎯 Business Problem
Financial institutions face major challenges due to:
- Highly **imbalanced transaction data**
- Increasing **UPI fraud cases**
- Need for **real-time fraud detection**
- High cost of **false negatives (missed frauds)**

## 🎯 Project Objective
- Build an ML model to classify UPI transactions as fraud / non-fraud  
- Improve detection of minority fraud class  
- Reduce false negatives using balanced learning  
- Compare model performance before and after SMOTE

## 📊 Dataset Description
- Type: UPI Transaction Dataset  
- Features:
  - Transaction amount  
  - Timestamp-based features  
  - User transaction behavior attributes  
- Target:
  - `0` → Legitimate Transaction  
  - `1` → Fraudulent Transaction  

## ⚙️ Tech Stack
**Programming Language:** Python 🐍  

**Libraries:**
- Pandas, NumPy → Data Processing  
- Scikit-learn → Machine Learning  
- Imbalanced-learn → SMOTE  
- Matplotlib / Seaborn → Visualization  

**Model Used:**
- Random Forest Classifier 🌲  

## 🔄 Project Workflow

### 1. Data Preprocessing
- Cleaned raw UPI dataset  
- Handled missing values  
- Removed irrelevant features  
- Created time-based features  

### 2. Handling Class Imbalance
- Dataset was highly imbalanced  
- Applied **SMOTE** to generate synthetic fraud samples  
- Balanced dataset improved learning ability  

### 3. Model Development
- Baseline Model: Random Forest (imbalanced data)  
- Optimized Model: Random Forest + SMOTE  

### 4. Train-Test Split
- 80% Training  
- 20% Testing  

## 🧠 Model Hyperparameters
- n_estimators = 100  
- max_depth = None  
- min_samples_split = 2  
- min_samples_leaf = 1  
- random_state = 42  
- bootstrap = True  
- SMOTE sampling_strategy = auto  

## 📈 Evaluation Metrics
- Accuracy Score  
- Precision  
- Recall (Critical for fraud detection)  
- F1-Score  
- Confusion Matrix  

## 📊 Results & Performance Analysis

### 🔴 Before SMOTE
- High accuracy but biased predictions  
- Poor fraud detection (low recall)  
- Model favored majority class  

### 🟢 After SMOTE
- Improved recall for fraud detection  
- Balanced classification performance  
- Better F1-score and confusion matrix distribution  

## 📌 Key Insights
- Class imbalance is a **major challenge in fraud detection systems**  
- SMOTE significantly improves minority class prediction  
- Random Forest performs strongly on structured financial data  
- Recall is more important than accuracy in fraud detection  

## 🚀 Final Outcome
The developed system successfully detects fraudulent UPI transactions and improves financial security by reducing undetected fraud cases using a balanced ML approach.

## 🔮 Future Enhancements
- Deployment using Flask / FastAPI (REST API)  
- Real-time fraud detection system  
- Integration with streaming data (Kafka / Spark)  
- Deep Learning models (LSTM, Autoencoders)  
- Feature engineering for higher accuracy  

## 👨‍💻 Highlights
✔ End-to-end ML pipeline implementation  
✔ Real-world fintech problem solved  
✔ Imbalanced dataset handling (SMOTE)  
✔ Model comparison & evaluation  
✔ Industry-relevant classification problem  

---

## 📍 Author
**Name:** Shaik Sumayya Sultana  
**Project:** UPI Fraud Detection System  
**Domain:** Machine Learning / FinTech    

## ⭐ Acknowledgements
Special thanks to open-source Python libraries and machine learning community for supporting this implementation.
