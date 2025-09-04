# 📱 Spam SMS Detection Using SVC + Tkinter

A machine learning project to classify SMS messages as **Spam** or **Ham (Not Spam)**.  
It uses a **Support Vector Classifier (SVC)** with **TF-IDF vectorization** and provides a **Tkinter-based GUI** for real-time message classification.

---

## ✨ Features

- ⚡ Detects whether an SMS is **Spam or Ham**.  
- 🧹 Performs **data cleaning** (lowercasing, removing punctuation, stopwords, etc.).  
- 🔎 Uses **TF-IDF vectorization** for feature extraction.  
- 🤖 Trains a **Support Vector Classifier (SVC)** achieving **97% accuracy**.  
- 🖥️ Includes a **Tkinter GUI** where users can enter SMS text and get predictions instantly.  
- 💾 Saves trained model & vectorizer (`svm_model.pkl`, `tfidf_vectorizer.pkl`) for reuse.

---

## 📂 Files in the Repository

- **spam.csv** → Dataset containing labeled SMS messages as spam/ham.  
  (Dataset source: [UCI SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection))  

- **training_and_model.py** → Main script:  
  - Cleans & preprocesses dataset  
  - Trains SVC + TF-IDF model  
  - Saves model/vectorizer as `.pkl`  
  - Launches Tkinter GUI for predictions  

- **svm_model.pkl** → Saved SVC model.  

- **tfidf_vectorizer.pkl** → Saved TF-IDF vectorizer.  

---

## ⚙️ How It Works

1. Load and preprocess dataset (`spam.csv`).  
2. Vectorize text using **TF-IDF**.  
3. Train a **Support Vector Classifier (SVC)**.  
4. Save trained model and vectorizer.  
5. Run **Tkinter GUI** → enter an SMS → model predicts **Spam/Ham** in real time.  

---

## 🛠️ Requirements

- Python 3.x  
- Libraries:  
  - scikit-learn  
  - pandas  
  - joblib  
  - os  
  - re  
  - tkinter (comes pre-installed with Python)  

Install dependencies:  

```bash
pip install scikit-learn pandas joblib
```

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/spam-sms-detection.git
   cd spam-sms-detection
