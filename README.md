# Fraud Detection System

## Project Overview
This project is a **fraud detection system** that uses **machine learning** to classify transactions as **fraudulent** or **legitimate**. The dataset used is the **Credit Card Fraud Detection Dataset**, and we apply **undersampling** to handle class imbalance.

## Features
- Data Preprocessing (Handling missing values, feature scaling, class balancing)
- Machine Learning Model (Random Forest)
- Model Evaluation (Precision, Recall, F1-score)
- Command-Line Interface (CLI) for testing new transactions

---

## 1. Installation & Setup
### **Prerequisites**
Make sure you have **Python 3.x** installed. You will also need the following Python libraries:

```bash
pip install pandas numpy scikit-learn
```

---

## 2. Dataset
Download the **credit_card_data.csv** dataset and place it in your project directory.

---

## 3. Running the Project
### **Step 1: Load and Preprocess Data**
The first step is to load the dataset, handle missing values and apply feature scaling. The class imbalance is handled using **Random Undersampling**.

### **Step 2: Train the Model**
A **Random Forest Classifier** ) is trained on the preprocessed dataset.

### **Step 3: Evaluate the Model**
After training, the model's performance is evaluated using:
- Classification Report (Precision, Recall, F1-score)

### **Step 4: Run the CLI for Fraud Detection**
Once the model is trained, you can test new transactions using the **Command-Line Interface (CLI)**.

Run the following command in your terminal or Jupyter Notebook:

```bash
python fraud_detection.py
```

---

## 4. Command-Line Interface (CLI) Usage
The CLI allows you to test transactions in two ways:

1️. **Manually enter transaction details**  
2️. **Use a random sample from the dataset**

When you run the program, you will see:

```bash
Choose Input Method:
1. Manually enter transaction details
2. Use a sample transaction from the dataset
Enter choice (1 or 2):
```

### Example Output
If you choose option 2 (random sample):

```bash
Using sample transaction from dataset:
[[ 0.75999676  0.23801765 -0.20441031 ... -0.90551162 -0.39625318]]

Prediction Result:
Legitimate Transaction.
```

If the model detects fraud, it will print:

```bash
Fraudulent Transaction Detected!
```

---

---

## 6. Notes
- Make sure to define `scaler` for feature scaling before using the CLI.
- If using **Jupyter Notebook**, ensure all code cells are executed before running the CLI.
- Modify the **train_test_split()** parameters if you want a different train-test split ratio.

---

## 7. Future Improvements
- Implement a **web interface** for user-friendly testing.
- Experiment with different **machine learning models**.
- Use **deep learning** (e.g., LSTMs) for better fraud detection.

---

This project is designed for learning purposes and demonstrates how to handle fraud detection using machine learning. Feel free to improve and expand it!

