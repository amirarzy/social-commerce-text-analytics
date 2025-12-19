# An Investigation on User Behavior in Social Commerce Platforms: A Text Analytics Approach

This project reproduces and extends an **academic study on user behavior in social commerce platforms** using text analytics and machine learning techniques.

The focus is on mining user‑generated content (reviews, comments, posts) to understand behavioral patterns, sentiments and key topics that drive engagement and purchase decisions.

---

## 📊 Problem & Data

- Goal: analyse how users interact with social commerce platforms through their textual content.  
- Typical data sources:
  - User reviews, comments or posts from a social commerce platform.  
  - Basic metadata such as user ID, timestamp, rating, product/category, etc.

The original academic work provides the conceptual framework; this implementation focuses on the **data and modeling pipeline** in Python. 
---

## 🧩 Text Preprocessing & Feature Engineering

Key steps in the pipeline:

- Text cleaning: lower‑casing, removing punctuation, stopwords, URLs and non‑informative tokens.  
- Tokenization and lemmatization / stemming to normalize word forms.  
- Feature extraction using:
  - Bag‑of‑Words / TF‑IDF representations.  
  - Optional n‑grams to capture short phrases.  
- Construction of document‑level features such as:
  - Review length, use of emotive words, rating information. 

These features are used for downstream tasks such as sentiment analysis, topic modeling and behavioral clustering.

---

## 🤖 Modeling & Analysis

Depending on the configuration, the project can include:

- **Sentiment analysis**:  
  - Supervised models (e.g. logistic regression, SVM) trained on labeled sentiment data.  
  - Evaluation with metrics such as accuracy, F1‑score, and confusion matrix.

- **Topic modeling**:  
  - Unsupervised models (e.g. LDA, NMF) to identify dominant themes in user discussions.  
  - Inspection of top words per topic and interpretation in terms of user behavior.

- **User segmentation**:  
  - Clustering users or documents based on text‑derived features to identify behavioral segments (e.g. bargain seekers, brand‑loyal users, highly engaged users). 

The notebook(s) document the full workflow from raw text to insights, mirroring the structure of the academic study.

---

## 📦 Outputs

Example outputs:

- Sentiment distribution for different product categories or user groups.  
- Topic summaries with representative keywords and example reviews.  
- Clusters / segments of users with descriptive statistics.

These insights can support:
- Marketing and personalization strategies.  
- Platform design decisions (UI/content changes).  
- Further research on social commerce behavior. 

---

## 🚀 How to Run

1. Prepare or download the text dataset (reviews/comments) and update the file paths in the notebook.  
2. Install dependencies:
  pip install pandas numpy scikit-learn nltk gensim
3. Open the main notebook in Jupyter / Colab and run all cells to:
- clean and preprocess text,  
- build features (TF‑IDF / n‑grams),  
- train and evaluate sentiment / topic models,  
- generate visualizations and tables with behavioral insights. 
