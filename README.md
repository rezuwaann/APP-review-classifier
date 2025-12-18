# 📱 Google Play Store App Review Classifier
**Author:** Rezuwan ahmed  <br>
**Tech Stack:** Python, Scikit-Learn, NLP, Logistic Regression  

## 📌 Project Overview
This project is a high-accuracy sentiment analysis tool designed to classify user feedback from the Google Play Store as **Positive** or **Negative**. By analyzing over 37,000 translated reviews, the model identifies key patterns in user satisfaction and app performance issues.

## 🎯 Key Presentation Points (TOC Structure)
Following the Theory of Computation (TOC) presentation guidelines, this project covers:

1. **Introduction:** Brief on NLP and the business impact of app feedback.
2. **Motivation:** Exploring binary sentiment classification in highly noisy real-world data.
3. **Problem Statement:** Transforming unstructured user "slang" and feedback into mathematical vectors for machine learning.
4. **Dataset & Pipeline:** * Dataset: 64,000+ raw rows (cleaned to ~37,000).
    * Pipeline: Handling Null values -> Case Folding -> TF-IDF Vectorization with N-grams.
5. **Methodology:** Comparison between Naive Bayes and Logistic Regression.
6. **Implementation:** Python-based environment using `scikit-learn` on Google Colab.
7. **Performance:** Achieving **~90% accuracy** through strategic data cleaning and Bigram analysis.
8. **Conclusion:** Insights into how specific keywords (e.g., "crash", "smooth") dominate app sentiment.

## 🛠️ The NLP Pipeline


To achieve the best accuracy, the following steps were taken:
* **Data Pruning:** Removed "Neutral" reviews to focus on strong sentiment signals.
* **Bigram Analysis:** Used `ngram_range=(1, 2)` to allow the model to understand context (e.g., "not working" vs just "working").
* **Logistic Regression:** Selected over Naive Bayes for better handling of feature correlations in large text datasets.

## 📊 Results & Performance
The model achieved high precision and recall, particularly in identifying negative reviews related to app bugs.

| Metric | Score |
| :--- | :--- |
| **Accuracy** | 90.15% |
| **Precision (Positive)** | 0.92 |
| **Recall (Positive)** | 0.94 |



## 🚀 Live Sample Predictions
| Review Text | Predicted Sentiment |
| :--- | :--- |
| "This app crashes every time I open the menu." | **Negative ❌** |
| "Absolutely beautiful UI and very fast transitions." | **Positive ✅** |
| "Not working after the latest update." | **Negative ❌** |
| "Best tool for my daily productivity!" | **Positive ✅** |

