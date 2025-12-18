# 🍽️ Restaurant Review Sentiment Classifier
**Author:** REZUWAN AHMED <br>
**Tech Stack:** Python, Scikit-Learn, Natural Language Processing (NLP)

## 📌 Project Overview
This project is a Machine Learning tool that automatically classifies restaurant reviews as **Positive** or **Negative**. Using Natural Language Processing (NLP) techniques, the model "reads" the text and understands customer satisfaction without human intervention.



## 🎯 Features
- **Data Cleaning:** Processes raw text by converting to lowercase and removing noise.
- **TF-IDF Vectorization:** Converts words into mathematical weights based on their importance.
- **Naive Bayes Classifier:** A powerful probabilistic model used for text classification.
- **Custom Prediction:** Includes a function to test the model with your own custom reviews.

## 📊 Dataset
The project uses the **Restaurant Reviews Dataset** from Kaggle, which consists of 1,000 reviews.
- **Target Variable:** `Liked` (1 = Positive, 0 = Negative).

## 📈 Model Performance
Based on the test data (20% of the dataset), the model achieved the following results:

| Metric | Score |
| :--- | :--- |
| **Accuracy** | 81.00% |
| **Precision (Positive)** | High |
| **Recall (Positive)** | High |



## 🚀 Live Samples
Here is how the model handles real-world sentences:

| Review | Predicted Sentiment |
| :--- | :--- |
| "The food was absolutely delicious and the service was fast!" | **Positive ✅** |
| "I hated the experience, the wait time was too long." | **Negative ❌** |
| "Crust is not good." | **Negative ❌** |
| "This place is amazing, I will come back again." | **Positive ✅** |


