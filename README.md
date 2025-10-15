🧠 Credit Card Fraud Detection (Unsupervised Learning)

📘 Overview
This project applies unsupervised learning techniques to detect anomalous (potentially fraudulent) transactions in a highly imbalanced credit card dataset.
Since labels were hidden during training, the models learned normal transaction behavior and later evaluated on real fraud labels.

📊 Project Overview
The dataset contains anonymized transaction features (`V1–V28`), along with `Amount`, `Time`, and a hidden `Class` label indicating fraud (1) or legitimate (0).  
The focus is on **detecting rare frauds** in highly imbalanced data.

🧰 Technologies Used
Python 3.10+
Libraries:
pandas, numpy, matplotlib, seaborn, plotly,
scikit-learn, tensorflow, keras

📊 Key Models
Isolation Forest:
Achieved low-to-medium precision and low recall. It primarily detects strong statistical outliers but may miss subtle fraud patterns.
One-Class SVM:
Performed similarly to Isolation Forest but showed slightly better recall. It is more sensitive to how features are scaled and can capture marginally finer distinctions.
Autoencoder:
Provided moderate precision but the best recall among the models. Its neural network structure allows it to learn complex, non-linear relationships, making it better at identifying subtle anomalies.
