# Spam SMS Detection Using SVC and Tkinter Interface

This project implements a spam SMS detection system using a Support Vector Classifier (SVC) with TF-IDF vectorization. It features a graphical user interface built with Tkinter for easy interaction.

---

## Files in the Repository

- **spam.csv**  
  The dataset containing labeled SMS messages as spam or ham. This dataset is also available on Kaggle: [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection)

- **training_and_model.py**  
  A single Python script that performs the entire workflow: data cleaning, model training using SVC and TF-IDF vectorizer, saving the trained model and vectorizer as `.pkl` files, and launching a Tkinter GUI for spam detection.

- **svm_model.pkl**  
  The trained SVC model saved using `joblib`.

- **tfidf_vectorizer.pkl**  
  The TF-IDF vectorizer saved using `joblib`.

---

## How It Works

1. Running `training_and_model.py` loads and cleans the dataset (`spam.csv`), then trains the SVC model with TF-IDF features.
2. The trained model and vectorizer are saved as `svm_model.pkl` and `tfidf_vectorizer.pkl`.
3. After training, a Tkinter GUI window opens where you can input SMS messages.
4. The GUI uses the saved model and vectorizer to classify messages as spam or ham in real-time.

---

## Requirements

- Python 3.x
- Libraries:
  - scikit-learn
  - pandas
  - joblib
  - os
  - re
  - tkinter (usually included with Python)

---

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/spam-sms-detection.git
   cd spam-sms-detection
