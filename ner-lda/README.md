### Assignment 1: Named Entity Recognition & Topic Modeling  
---

## 🧠 Task 1: Named Entity Recognition

- **Model:** [e.g., CRF / BiLSTM / Logistic Regression]  
- **Features:** Token, lowercase, prefix/suffix, POS tags, context tokens  
- **Metrics:** Precision, Recall, F1  
- **Tools:** nltk, sklearn, sklearn-crfsuite  

---

## 🗂️ Task 2: Topic Modeling

- **Steps:** Text cleaning → Lemmatization → POS filtering → LDA  
- **Libraries:** spaCy, gensim, wordcloud  
- **Topics:** Top 5 with keywords, coherence score (e.g., `c_v`)  
- **Visualization:** Word clouds for each topic  

---

## ▶️ Run Instructions

```bash
pip install nltk spacy gensim wordcloud scikit-learn
python -m nltk.downloader all
python -m spacy download en_core_web_sm
