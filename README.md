# 🛡️ Network Traffic Analysis for Intrusion System: Detection of Specific Attacks

This project focuses on developing a Machine Learning-based **Intrusion Detection System (IDS)** capable of accurately distinguishing between **normal and malicious network traffic**, with a focus on specific attack types such as **DDoS**, **Brute Force**, and **SQL Injection**.

---

## 🎯 Objectives

- 🔍 To develop an IDS that utilizes **Deep Neural Networks (DNNs)** to classify network traffic as normal or malicious.
- ⚖️ To apply **Conditional Generative Adversarial Networks (cGANs)** for **data augmentation**, improving class balance in the dataset.
- 🧠 To implement **SHAP (SHapley Additive Explanations)** for **model interpretability** and feature importance analysis.
- 📊 To evaluate performance using key metrics: **Accuracy, Precision, Recall, and F1-Score**.

---

## 🧰 Technologies Used

- 🐍 Python 3
- 📓 Jupyter Notebook (via VS Code extension)
- 🔁 cGANs (Conditional Generative Adversarial Networks)
- 🤖 Deep Neural Networks (DNNs)
- 🧠 SHAP (Explainable AI - XAI)
- 📦 Libraries: `TensorFlow`, `Keras`, `pandas`, `scikit-learn`, `matplotlib`, `SHAP`, `NumPy`

---

## 🛠️ Features

- ✅ Data Preprocessing: Cleaning, encoding, scaling, and transformation of CICIDS2018 dataset.
- 🧬 Data Augmentation using cGANs to handle class imbalance (e.g., underrepresented attack types).
- 📈 DNN-based classification model trained on balanced and imbalanced datasets.
- 🔍 SHAP analysis to interpret model predictions and understand key influencing features.
- 📊 Evaluation using confusion matrix, precision, recall, accuracy, and F1-score.

---

## 📁 Project Structure

```bash
FYP-NIDS/
│
├── notebooks/
│   ├── 1_preprocessing.ipynb            ← Data cleaning, transformation
│   └── 2_dnn_cgan_shap.ipynb            ← Model training, augmentation, SHAP
│
├── data/
│   ├── CICIDS2018/                      ← Folder for raw data splits
│   ├── merged.csv                       ← Combined full dataset
│   └── preprocessed.csv                 ← Cleaned/encoded/scaled version
│
├── images/                              ← Plots, SHAP, confusion matrix
│   ├── shap_summary.png
│   └── confusion_matrix.png
│
├── models/                              ← Saved model files
│   └── dnn_model.h5
│
├── requirements.txt
├── README.md
└── .gitignore

```

## 🧾 Dataset: CICIDS2018

The project uses the [CICIDS2018 dataset](https://www.unb.ca/cic/datasets/ids-2018.html) by the Canadian Institute for Cybersecurity.

This dataset contains realistic network traffic data including both benign and malicious activity, such as:

- DDoS
- Brute Force (SSH/FTP)
- SQL Injection
- Botnet, PortScan, and more

**Preprocessing includes**:
- Merging all day-wise CSV files into a single dataset
- Dropping null and duplicate rows
- Encoding categorical values
- Feature scaling
- Splitting for training and testing

A final preprocessed dataset is saved as:  
`data/preprocessed.csv`
