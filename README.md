# 📰 Fake News Detection using NLP & Machine Learning

## 🎯 Executive Summary & Project Proposal
The rapid spread of fake news is a major problem because it deliberately manipulates public opinion, fuels polarisation, and undermines trust in democratic institutions. 

**The Objective:** To automate the detection of fabricated content by analysing linguistic patterns and semantic inconsistencies, enabling real-time classification of news as "real" or "fake" to protect platform integrity.

## 🛠️ Methodology & Tech Stack
This project features an end-to-end Natural Language Processing (NLP) pipeline built in Python:
* **Data Wrangling:** Cleaned a 40,000+ article dataset using `pandas`, handling missing values and dropping duplicates (Exploratory Data Analysis).
* **Text Preprocessing:** Utilised `nltk` and Regular Expressions to remove noise (punctuation, URLs), filter stopwords, and apply Lemmatisation to extract root meanings.
* **Feature Engineering:** Transformed raw text into mathematical sparse matrices using **TF-IDF** (Term Frequency-Inverse Document Frequency) via `scikit-learn`.
* **Machine Learning:** Trained, evaluated, and compared two classification models: **Logistic Regression** and **Random Forest**.

## 📊 Key Results & Business Impact
We evaluated the models using Classification Reports and Confusion Matrices, prioritising **Precision** to ensure the platform does not accidentally censor legitimate, real news (False Positives).

🏆 **Winning Model: Random Forest**
* **High Precision:** Out of over 4,700 actual *Real* news articles in the test set, the Random Forest model only misclassified 38 of them. 
* **Conclusion:** The Random Forest successfully minimised catastrophic False Positives while maintaining high accuracy in catching truly fabricated articles, successfully balancing platform safety with journalistic integrity.

## 🚀 How to Run this Project
1. Clone this repository to your local machine.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Download ISOT Fake News Dataset 
4. Open the Jupyter Notebook (`.ipynb` file) to view the code, visualisations, and model training steps.
