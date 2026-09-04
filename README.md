# NLP-Based Spam Message Detection Using TF-IDF and Machine Learning

##  Project Overview

This project is an NLP-based machine learning system designed to automatically classify SMS messages as **Spam** or **Ham**.

The system applies Natural Language Processing techniques to clean and preprocess SMS text, converts the text into numerical features using **TF-IDF**, and uses machine learning algorithms to classify messages.

Two machine learning models were implemented and compared:

* Multinomial Naive Bayes
* Logistic Regression

The **Multinomial Naive Bayes** model achieved the best performance with an accuracy of **97.04%**.

---

##  Objectives

* Develop an NLP-based SMS spam detection system.
* Preprocess SMS text using NLP techniques.
* Extract text features using TF-IDF.
* Train machine learning models for classification.
* Compare Multinomial Naive Bayes and Logistic Regression.
* Evaluate model performance using standard classification metrics.
* Predict whether new SMS messages are Spam or Ham.

---

##  Dataset

The project uses an SMS spam classification dataset containing **5,572 messages**.

| Category  | Number of Messages |
| --------- | -----------------: |
| Ham       |              4,825 |
| Spam      |                747 |
| **Total** |          **5,572** |

### Dataset Attributes

* `label` – Target class: Ham or Spam
* `message` – Text content of the SMS

The dataset is included in the `dataset/` folder of this repository.

---

##  NLP Preprocessing

The following preprocessing steps were applied:

1. Convert text to lowercase.
2. Remove URLs.
3. Remove numbers.
4. Remove punctuation.
5. Tokenize the text.
6. Remove English stopwords.
7. Remove very short words.

---

##  Feature Extraction

**TF-IDF (Term Frequency-Inverse Document Frequency)** was used to convert text messages into numerical feature vectors.

The implementation used:

* Maximum features: 5,000
* N-gram range: 1–2

This allows the system to consider both individual words and two-word combinations.

---

##  Machine Learning Models

### 1. Multinomial Naive Bayes

Multinomial Naive Bayes was selected because it is efficient and well suited for text classification problems.

### 2. Logistic Regression

Logistic Regression was implemented as a second model to compare classification performance.

---

##  Results

| Model                       |   Accuracy |   Precision |     Recall |   F1 Score |
| --------------------------- | ---------: | ----------: | ---------: | ---------: |
| **Multinomial Naive Bayes** | **97.04%** | **100.00%** | **77.85%** | **87.55%** |
| Logistic Regression         |     96.95% |     100.00% |     77.18% |     87.12% |

###  Best Model

**Multinomial Naive Bayes** was selected as the final model because it achieved the highest accuracy and F1-score among the tested models.

---

##  Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* NLTK
* Scikit-learn
* Matplotlib
* Seaborn

---

##  Project Structure

```text
NLP-Spam-Detection/
│
├── README.md
├── source_code.py
├── requirements.txt
│
├── dataset/
│   └── spam.csv
│
├── screenshots/
│   ├── dataset.png
│   ├── preprocessing.png
│   ├── confusion_matrix.png
│   ├── model_comparison.png
│   └── results.png
│
└── report/
    └── NLP_Spam_Detection_Report.pdf
```

---

## 📸 Screenshots

Screenshots of the dataset, preprocessing, confusion matrix, model comparison, and final results are available in the `screenshots/` folder.

---

##  Limitations

* The dataset contains fewer spam messages than ham messages.
* The dataset may not represent all modern spam patterns.
* The system primarily focuses on English SMS messages.
* TF-IDF does not fully capture contextual meaning.
* New spam patterns may require additional training data.

---

##  Future Scope

* Use larger and more recent datasets.
* Support multiple languages.
* Implement advanced NLP models such as BERT.
* Develop a web or mobile application.
* Enable real-time spam detection.
* Continuously update the model with new spam examples.
* Improve detection of evolving spam patterns.

---

##  Conclusion

The project demonstrates how Natural Language Processing and machine learning can be used to automatically detect SMS spam.

Using TF-IDF features, both Multinomial Naive Bayes and Logistic Regression achieved high classification performance. Multinomial Naive Bayes achieved the best result with **97.04% accuracy** and an **87.55% F1-score**, making it the selected model for the final spam detection system.

---

## 👨‍💻 Project

**NLP Mini Project – Spam Message Detection**

Developed using Python, NLTK, TF-IDF, and Machine Learning.

