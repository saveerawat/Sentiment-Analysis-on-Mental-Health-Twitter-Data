# Sentiment-Analysis-on-Mental-Health-Twitter-Data
**1. Project Overview**

This project analyzes 20,000 mental-health–related tweets to detect depression indicators using text sentiment and machine learning.

**2. Dataset**

Columns: post_text, id, user_id, post_created, label (depressed / not depressed)<br>
Main features used: post_text, label

**3. Data Cleaning & Preprocessing**

i. Removed punctuations and numbers<br>
ii. Removed stopwords & performed tokenization (NLTK / spaCy)

**4. Sentiment Analysis (TextBlob)**

- Polarity: −1 (negative) → +1 (positive)
- Subjectivity: <0.5 factual, >0.5 personal opinion
- Created a sentiment (positive/negative) column from polarity scores

**5. Machine Learning Model**

Decision Tree Classifier<br>
Train-test split:<br>
X = post_text<br>
Y = sentiment<br>

- Converted text into numerical vectors using CountVectorizer.<br>
- Achieved 94% accuracy (with high precision, recall, F1-score)
