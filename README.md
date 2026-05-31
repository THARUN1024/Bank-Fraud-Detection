# 🏦 Bank Fraud Detection using SQL

Dataset : https://www.kaggle.com/datasets/ealaxi/paysim1

## 📌 Project Overview

This project focuses on detecting fraudulent banking transactions using SQL. The project leverages a transactional dataset to perform comprehensive Exploratory Data Analysis (EDA), identify fraudulent activities, and generate actionable insights.

By analyzing transaction patterns, balance inconsistencies, and transaction types, this project demonstrates how SQL can be effectively used for fraud detection in banking systems.

---

## 📂 Dataset

The dataset contains banking transaction records with the following fields:

- **step** – Time step (in hours) from the start of data collection
- **type** – Type of transaction (e.g., CASH_OUT, TRANSFER, PAYMENT, DEBIT)
- **amount** – Transaction amount
- **nameOrig** – Sender's customer ID
- **oldbalanceOrg** – Sender's balance before transaction
- **newbalanceOrig** – Sender's balance after transaction
- **nameDest** – Receiver's customer ID
- **oldbalanceDest** – Receiver's balance before transaction
- **newbalanceDest** – Receiver's balance after transaction
- **isFraud** – Fraud indicator (1 = Fraudulent, 0 = Legitimate)

---

## 🎯 Objectives

- Detect fraudulent transactions using SQL.
- Analyze transaction behavior and fraud patterns.
- Identify transaction types most susceptible to fraud.
- Discover anomalies in account balances.
- Generate actionable insights from transactional data.

---

## 🛠️ Tools Used

- SQL (MySQL / PostgreSQL)
- MySQL Workbench
- pgAdmin
- Excel / CSV Viewer

---

## 📁 Repository Structure

```text
Bank_Fraud_Detection_SQL/
│
├── Bank_fraud_detection.sql    # SQL queries and analysis
├── Dataset.csv                 # Transaction dataset
└── README.md                   # Project documentation
```

---

## 🔍 Key SQL Operations

- Data cleaning and preprocessing
- Fraud transaction filtering
- Aggregation and grouping analysis
- Balance consistency checks
- Time-based transaction analysis
- Fraud pattern identification
- Creation of fraud detection flags

### SQL Concepts Applied

- SELECT
- WHERE
- GROUP BY
- ORDER BY
- HAVING
- CASE Statements
- Aggregate Functions
- Subqueries
- Window Functions

---

## 🚨 Fraud Detection Logic

The project identifies suspicious transactions using the following business rules:

### 1. Suspicious Transaction Types

Fraud is primarily associated with:

- CASH_OUT
- TRANSFER

### 2. Balance Inconsistencies

Transactions where:

- Sender's balance does not decrease correctly.
- Receiver's balance does not increase correctly.

### 3. High-Value Transactions

- Large transfers executed within short time intervals.
- Unusually high transaction amounts compared to normal behavior.

### 4. Repeated Fraud Destinations

- Destination accounts frequently involved in fraudulent transactions.

---

## 📊 Analysis Performed

### Transaction Type Analysis

- Distribution of transactions by type.
- Fraud occurrence by transaction type.

### Fraud Distribution

- Total fraudulent vs non-fraudulent transactions.
- Fraud percentage across transaction categories.

### Balance Verification

- Validation of sender and receiver balances.
- Identification of balance anomalies.

### Destination Account Analysis

- Most common fraud destination accounts.
- Frequency of fraudulent transactions per destination.

### Time-Based Analysis

- Fraud occurrence across different time steps.
- Peak periods of fraudulent activity.

---

## 📈 Key Insights

- The majority of fraudulent transactions occur in **TRANSFER** and **CASH_OUT** transaction types.
- Fraudulent transactions frequently exhibit balance update inconsistencies.
- Certain destination accounts repeatedly appear in fraud cases.
- High-value transfers are more likely to be associated with fraudulent activity.
- Transaction behavior patterns can be effectively identified using SQL-based analysis.

---

## ✅ Project Highlights

- End-to-end fraud analysis using SQL.
- Real-world banking transaction dataset.
- Fraud detection based on business rules and transaction behavior.
- Use of advanced SQL concepts including CASE statements and Window Functions.
- Generation of actionable fraud-related insights.

---

## 🧠 Learning Outcomes

Through this project, I gained hands-on experience in:

- SQL-based data analysis
- Exploratory Data Analysis (EDA)
- Fraud detection techniques
- Writing complex SQL queries
- Business logic implementation in SQL
- Transaction pattern analysis
- Data-driven decision making

---

## 📌 Conclusion

This project demonstrates how SQL can be used not only for data retrieval but also for identifying fraudulent financial activities. By analyzing transaction patterns, balance inconsistencies, and account behaviors, valuable fraud-related insights can be extracted to support risk management and fraud prevention efforts.
