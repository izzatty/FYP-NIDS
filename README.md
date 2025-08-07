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
├── data/                   # CICIDS2018 or processed datasets
├── cgan/                   # Code for training cGAN
├── dnn_model/              # DNN training and evaluation scripts
├── shap_analysis/          # SHAP interpretability visualizations
├── results/                # Model metrics and graphs
├── requirements.txt        # Python dependencies
├── README.md               # Project overview
