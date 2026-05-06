# Fake News Stance Detection Using Natural Language Processing and Machine Learning

## Project Overview

This project applies Natural Language Processing (NLP) and machine learning techniques to detect the stance of news article headlines relative to news article bodies.

The system classifies whether a headline:

- Agrees with the article
- Disagrees with the article
- Discusses the article
- Is unrelated to the article

The project focuses on text preprocessing, feature engineering, vectorisation, machine learning classification, and stance prediction.

The aim is to explore how NLP can assist in misinformation analysis and automated fake news detection systems.

---

## Dataset

The dataset contains news headlines and corresponding article bodies.

Main files include:

- `train_bodies.csv`
- `train_stances.csv`
- `test_bodies.csv`
- `competition_test_bodies.csv`
- `competition_test_stances.csv`
- `competition_test_stances_unlabeled.csv`

Target classes:

- `agree`
- `disagree`
- `discuss`
- `unrelated`

---

## Project Objectives

- Preprocess textual news data
- Clean and tokenize text
- Extract NLP features
- Transform text into numerical representations
- Train and evaluate stance classification models
- Analyse model performance across stance categories
- Investigate fake news detection challenges

---

## Natural Language Processing Techniques

The project includes:

- Text cleaning
- Lowercasing
- Stopword removal
- Tokenisation
- TF-IDF Vectorisation
- Feature extraction
- Text similarity analysis

---

## Machine Learning Models Used

The following models were trained and evaluated:

- Logistic Regression
- Naive Bayes
- Random Forest Classifier
- Support Vector Machine (SVM)
- XGBoost Classifier

---

## Evaluation Metrics

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

---

## Key Challenge: Class Imbalance

One of the major challenges in stance detection is class imbalance.

The `unrelated` class is often dominant, which can cause machine learning models to achieve high overall accuracy while performing poorly on minority stance categories such as `agree` or `disagree`.

This project investigates how different models behave under these imbalance conditions.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Natural Language Processing (NLP)
- TF-IDF Vectorisation
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/your-username/fake-news-stance-detection.git
```

### 2. Open the project directory

```bash
cd fake-news-stance-detection
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open and run the notebook

Run:

```text
main.ipynb
```

from top to bottom.

---

## Repository Structure

```text
.
├── main.ipynb
├── train_bodies.csv
├── train_stances.csv
├── test_bodies.csv
├── test_stances_unlabeled.csv
├── competition_test_bodies.csv
├── competition_test_stances.csv
├── competition_test_stances_unlabeled.csv
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Key Insights

- Text preprocessing significantly affected model performance.
- TF-IDF vectorisation provided effective numerical representations of text.
- Class imbalance impacted minority stance prediction quality.
- Simpler linear models performed competitively on sparse text data.

---

## Future Improvements

- Use transformer-based NLP models such as BERT
- Apply deep learning architectures
- Improve handling of class imbalance
- Add semantic similarity techniques
- Build a real-time fake news analysis web app
- Deploy the system using Streamlit or Flask

---

## .gitignore

```text
.ipynb_checkpoints/
__pycache__/
*.pyc
.DS_Store
.env
venv/
```

---

## Author

Uvietobore Joshua Adjugah

MSc Data Science and Artificial Intelligence
