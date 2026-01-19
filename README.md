🔐 Network Intrusion Detection System using NSL-KDD Dataset
📌 Project Overview

This project focuses on building a Network Intrusion Detection System (NIDS) using the NSL-KDD dataset. The goal is to classify network connections as normal or malicious by applying data preprocessing, feature engineering, and machine learning techniques.

The project demonstrates how real-world network traffic data can be analyzed and transformed into a structured format suitable for binary and multi-class classification tasks.

🎯 Problem Statement

Modern networks are vulnerable to various cyber attacks such as DoS, Probe, R2L, and U2R.
The objective of this project is to:

Detect whether a network connection is normal or an attack

Identify different types of attacks using machine learning models

📂 Dataset Description

The NSL-KDD dataset is an improved version of the KDD’99 dataset and is widely used for intrusion detection research.

Each row represents a network connection

Total 41 features + 1 label column

Each record describes how data flows between two systems

🎯 Target Labels

Binary Classification

0 → Normal Traffic

1 → Attack Traffic

Multi-class Classification

Normal

DoS (Denial of Service)

Probe

R2L (Remote to Local)

U2R (User to Root)

🧾 Feature Types
🔢 Numerical Features

Describe measurable network properties:

duration – connection duration

src_bytes – data sent from source

dst_bytes – data received by destination

These features capture traffic size, speed, and behavior.

🏷️ Categorical Features

Describe the nature of the connection:

protocol_type – TCP, UDP, ICMP

service – HTTP, FTP, SMTP, etc.

flag – connection status

These features are encoded before model training.

🛠️ Data Preprocessing

To prepare the dataset for machine learning, the following steps were applied:

Categorical Encoding

One-hot encoding for protocol type, service, and flag

Data Cleaning

Converted all features to numerical format

Handled missing values using safe defaults

Feature Scaling

Applied StandardScaler to normalize feature ranges

Improved performance of linear models

Feature Selection

Used Random Forest feature importance

Selected top contributing features to reduce complexity

Train–Test Split

Stratified split to maintain class distribution

Separate training and testing datasets

🤖 Machine Learning Approach

Supervised learning techniques applied

Feature importance used to improve efficiency

Supports both binary and multi-class classification tasks

📊 Evaluation

Model performance is evaluated on unseen test data to ensure:

Accurate attack detection

Reduced false positives

Better generalization

🧰 Tech Stack

Language: Python

Libraries:

Pandas

NumPy

Scikit-learn

Matplotlib / Seaborn

Environment: Jupyter Notebook

🚀 Future Enhancements

Apply advanced models like Random Forest, XGBoost, or Neural Networks

Perform real-time intrusion detection

Deploy as a security monitoring dashboard

🏁 Conclusion

This project demonstrates how proper data preprocessing, feature selection, and machine learning techniques can be used to build an effective intrusion detection system. It highlights the importance of transforming raw network traffic into meaningful features for accurate attack detection.
