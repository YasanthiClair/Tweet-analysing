# Airline Tweet Sentiment Analysis ✈️📊

This repository contains a machine learning project focused on Natural Language Processing (NLP) to classify the sentiment of tweets directed at various airlines. The goal is to preprocess raw text data and accurately predict whether an airline tweet expresses a **positive**, **neutral**, or **negative** sentiment.

---

## 🚀 Key Features & Workflow

The project is implemented in a Jupyter Notebook (`airplane_tweet.ipynb`) and follows a structured data science pipeline:

1. **Data Loading & Filtering:** * Loads the airline tweets dataset using `pandas`.
   * Filters out unnecessary data to focus strictly on `airline_sentiment` and the raw `text`.

2. **Text Preprocessing:**
   * Converts text to lowercase and removes URLs using regular expressions (`re`).
   * Tokenizes text using `nltk.word_tokenize`.
   * Removes standard English stopwords and punctuation marks.
   * Applies **Porter Stemming** (`PorterStemmer`) to reduce words to their base or root form.

3. **Feature Extraction:**
   * Transforms the cleaned text data into numerical features using **TF-IDF Vectorization** (`TfidfVectorizer`) with a maximum of 3,000 top features.

4. **Model Training & Evaluation:**
   * Splits the data into an 80/20 train-test split (`train_test_split`).
   * Evaluates and compares multiple classification models.

---

## 🛠️ Tech Stack & Libraries

* **Language:** Python
* **Data Manipulation:** Pandas
* **Natural Language Processing:** NLTK
* **Machine Learning:** Scikit-learn
  * `TfidfVectorizer` (Feature Engineering)
  * `MultinomialNB` (Naive Bayes)
  * `RandomForestClassifier` (Ensemble Learning)

---

## 📈 Model Performance Results

The models were evaluated using classification accuracy scores on the testing set:

| Machine Learning Model | Testing Accuracy |
| :--- | :--- |
| **Naive Bayes (MultinomialNB)** | 72.2% |
| **Random Forest Classifier** | **75.0%** 🏆 |

*The Random Forest Classifier provided the highest predictive accuracy for sentiment classification on this dataset.*

---

## 💻 How to Run the Project

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YasanthiClair/Tweet-analysing.git](https://github.com/YasanthiClair/Tweet-analysing.git)
   cd Tweet-analysing
