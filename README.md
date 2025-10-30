# 🧠 Hate Speech and Offensive Language Detection Using Machine Learning

## Overview
This project focuses on detecting and classifying **hate speech**, **offensive language**, and **neutral content** from social media text using Natural Language Processing (NLP) and Machine Learning techniques.  
With the rapid growth of user-generated content online, effective content moderation is essential to maintain safe and inclusive communication platforms.  
The model categorizes text into predefined classes, supporting responsible social media management and reducing exposure to harmful content.

---

## Problem Statement
Accurately identifying harmful language is a complex challenge due to contextual nuances — a phrase may be offensive in one context but harmless in another.  
The goal of this project is to build a **robust and interpretable NLP model** that can classify tweets or short text messages into three categories:
- **Hate Speech**
- **Offensive Language**
- **Neutral Content**

This solution supports automated content moderation, enhancing platform integrity and user safety.

---

## Dataset
- **Source:** Publicly available dataset of labeled tweets for hate speech and offensive language classification.  
- **Records:** 24,783 labeled tweets.  
- **Format:** CSV file with text and associated labels.

### **Class Labels**
| Label | Description |
|--------|-------------|
| Hate Speech | Contains hate or discriminatory expressions |
| Offensive Language | Contains offensive words but not categorized as hate speech |
| Neutral | Non-offensive and neutral statements |

### **Key Variables**
- **count** – total number of classifications assigned to each tweet  
- **hate_speech, offensive_language, neither** – number of votes each tweet received per category  

---

## 🧰 Tools & Technologies
- Python (3.10+)  
- Pandas, NumPy  
- NLTK, Scikit-learn  
- TextBlob, WordCloud  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## Methodology

### 1. Text Preprocessing
- Converted text to lowercase  
- Removed punctuation, stopwords, URLs, and special characters  
- Tokenized and lemmatized text  
- Encoded categorical labels for supervised learning  

### 2. Feature Engineering
- Extracted features using **TF-IDF Vectorization**  
- Visualized most frequent and impactful words using **WordClouds**  
- Explored n-grams and term distributions for linguistic insight  

### 3. Model Development
- Implemented and compared multiple models:
  - Logistic Regression  
  - Multinomial Naïve Bayes  
  - Support Vector Machine (SVM)  
  - Random Forest Classifier  
- Used an 80/20 train-test split for model evaluation.  

### 4. Evaluation Metrics
- **Accuracy**, **Precision**, **Recall**, **F1-Score**  
- **Confusion Matrix** for multi-class performance visualization  
- **ROC–AUC** for overall discriminative power  

---

## 📊 Results
| Model | Accuracy | F1-Score | Notes |
|--------|-----------|----------|-------|
| Logistic Regression | 0.88 | 0.86 | Reliable baseline performance |
| Naïve Bayes | 0.84 | 0.82 | Performs well with sparse text data |
| SVM | **0.90** | **0.89** | Best model for balanced precision and recall |

**Key Insights**
- Most tweets were neutral or mildly offensive, while hate speech represented the smallest portion.  
- The **SVM model** achieved the highest accuracy and recall, effectively reducing false negatives.  
- Text preprocessing and TF-IDF feature extraction significantly improved classification accuracy.  

---

## 🌍 Visualizations
- **WordCloud:** Displays most frequent offensive terms  
- **Confusion Matrix:** Shows per-class prediction performance  
- **Bar Plot:** Visualizes class distribution of predictions  

![WordCloud Example](images/hate_speech_wordcloud.png)

---

## 🚀 Future Enhancements
- Integrate **deep learning models (BERT, RoBERTa, or LSTM)** for contextual understanding.  
- Deploy the model through **Streamlit** or **Flask** for real-time moderation.  
- Expand to **multi-language** detection and large-scale social media datasets.  

---

## 👩‍💻 Author
**Pria Khatik**  
M.S. in Artificial Intelligence & Business Analytics, University of South Florida  

🔗 [LinkedIn – Pria Khatik](https://www.linkedin.com/in/priyakhatik/)  
📅 *2025 | NLP & Machine Learning Project*

---
