# Fraud Classification for Financial Transactions
This project aims to detect fraudulent transactions in financial datasets using machine learning. It implements multiple algorithms, including KNN, RFC, and Decision Trees, and optimizes them through hyperparameter tuning. The model evaluates accuracy, precision, and recall for effective fraud detection.


## 📌 Project Overview
This project focuses on detecting fraudulent financial transactions using machine learning techniques. Fraudulent transactions pose a significant risk to businesses and consumers, making it crucial to develop accurate and efficient fraud detection models.

By leveraging machine learning algorithms, this project identifies patterns and anomalies in transaction data to differentiate fraudulent activities from legitimate ones. The ultimate goal is to build a robust predictive model that can be integrated into financial security systems to help prevent fraud and minimize financial losses.

## 📂 Dataset
The dataset contains multiple features related to financial transactions. The key attributes are:

| Column Name            | Description |
|------------------------|-------------|
| `Time`                 | Time of the transaction since the first transaction in the dataset |
| `V1 to V28`            | Principal components derived from PCA to capture hidden structures in the data |
| `Amount`               | Transaction amount |
| `Class`                | Target variable, where **0** represents non-fraudulent transactions and **1** represents fraudulent transactions |

## 🔎 Data Processing Workflow

### 1️⃣ **Exploratory Data Analysis (EDA)**
- Visualizing distributions using histograms and box plots.
- Identifying missing values, duplicates, and anomalies.
- Analyzing class imbalance between fraudulent and non-fraudulent transactions.

### 2️⃣ **Feature Engineering & Preprocessing**
- Handling missing values and removing duplicate transactions.
- Normalizing numerical features (`Amount` and `Time`) to ensure consistency.
- Addressing class imbalance using oversampling techniques such as **SMOTE**.

### 3️⃣ **Model Development & Evaluation**
- Implementing multiple machine learning models for classification:
  - ✅ K-Nearest Neighbors (KNN)
  - ✅ Decision Trees
  - ✅ Random Forest
  
- Optimizing hyperparameters using **RandomizedSearchCV**.
- Evaluating models using performance metrics:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **F1-score**

### 4️⃣ **Feature Importance & Interpretability**
- Analyzing feature importance to understand key indicators of fraudulent activity.
- Evaluating decision boundaries of different models to interpret fraud detection strategies.
- Assessing the impact of balancing techniques on classification performance.

## 🚀 How to Run the Project

### **1️⃣ Clone the Repository**
```sh
$ git clone https://github.com/yourusername/Fraud-Classification.git
$ cd Fraud-Classification
```

### **2️⃣ Install Dependencies**
```sh
$ pip install -r requirements.txt
```

### **3️⃣ Run the Jupyter Notebook**
```sh
$ jupyter notebook
```
Open the `Fraud_Classification.ipynb` file and execute the cells.

## 📊 Results
- The best-performing model achieved a high **accuracy**, with precision and recall optimized for identifying fraudulent transactions.
- Features such as **transaction amount, time, and PCA components** played a significant role in detecting fraudulent activities.
- The model successfully minimizes false positives while maximizing fraud detection accuracy.

## 📌 Future Improvements
- 🔹 Implementing **real-time transaction monitoring** for enhanced fraud detection.
- 🔹 Exploring **deep learning models** such as **LSTMs** and **Autoencoders** for anomaly detection.
- 🔹 Deploying the fraud detection model as a **REST API** for seamless integration with financial systems.


## 🔚 Conclusion
This project provides an effective machine learning-based approach to detecting fraudulent transactions in financial datasets. By identifying key patterns and anomalies, the model helps financial institutions reduce fraud-related losses. Future enhancements, such as deep learning and real-time monitoring, will further improve the accuracy and practicality of the fraud detection system.



