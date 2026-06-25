# Disaster Tweets — NLP Classification 🌪️

My first machine learning project. Built a complete NLP pipeline
to classify tweets as disaster or not disaster.

**Competition:** Kaggle — Natural Language Processing with Disaster Tweets
**Public Score:** 0.79037 (F1)
**Notebook:** [View on Kaggle](https://www.kaggle.com/code/muskangait/muskan-gait)

---

## About This Project

I am a beginner learning AI and ML from scratch. This is my first
complete machine learning project where I built everything step by step
and documented my learning process including errors I made along the way.

---

## What I Built

Starting from raw noisy tweets I built everything from scratch:

- EDA to understand class balance, missing values, tweet lengths
- 7 step text cleaning pipeline that removed 43.8% noise
- TF-IDF vectorization with 5000 features + 3 metadata features
- Trained and compared 3 models
- Submitted predictions to Kaggle leaderboard

---

## Results

| Model | Validation F1 |
|-------|--------------|
| Logistic Regression | 0.7914 |
| Naive Bayes | 0.8100 ← best |
| Random Forest | 0.7735 |

**Public Leaderboard Score: 0.79037**

---

## Errors I Made Along the Way

I documented every error because mistakes are the best learning moments.

**Error 1 — FileNotFoundError**
Did not know Kaggle needs manual dataset attachment.
Fixed by learning how Kaggle input paths work.

**Error 2 — NLTK download blocked**
Kaggle blocked external downloads.
Fixed by pointing NLTK to pre-installed data at /usr/share/nltk_data

**Error 3 — KeyError on test dataframe**
Created length features on train but forgot test dataframe.
Fixed by adding same feature creation for test.
Most important lesson — train and test are completely separate objects.

---

## What I Learned

- Same word can mean completely different things in different context
- Nearly half of every tweet is noise — cleaning matters more than model
- Naive Bayes works surprisingly well on text classification
- Sparse matrices reduce memory from 304MB to 503KB — 600x reduction
- Always check class balance before choosing evaluation metric
- Document your errors — they teach more than smooth runs

---

## What I Would Improve Next Time

- Use lemmatization instead of stemming
- Add URL presence as binary feature
- Try SVM classifier
- Use cross validation instead of single train/val split
- Try BERT for better contextual understanding

---

## Tech Stack
Python | Pandas | NumPy | Matplotlib | Seaborn | NLTK | Scikit-learn



