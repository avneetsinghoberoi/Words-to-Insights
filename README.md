# Words to Insights

This project demonstrates a complete end-to-end **Text Mining** pipeline using a custom dataset of 20 sample documents (product reviews or user comments). It includes preprocessing, word cloud visualization, topic modeling with LDA, and sentiment analysis.

---

## 📋 Features

- ✅ Sample dataset with 20 textual reviews
- ✅ Text preprocessing (cleaning, stopwords, lemmatization)
- ✅ Word Cloud for text visualization
- ✅ Topic Modeling using LDA (Latent Dirichlet Allocation)
- ✅ Sentiment analysis using TextBlob
- ✅ Sentiment classification and distribution plot

---

## 📁 Dataset

- 20 textual documents
- Each row represents a short customer review
- Stored in a simple Pandas DataFrame with columns: `doc_id`, `text`

---

## 🛠 Tools & Libraries

- `pandas`, `numpy`
- `nltk`, `textblob`
- `scikit-learn` (LDA, Vectorizers)
- `matplotlib`, `seaborn`
- `wordcloud`

---

## Execution Flow

### 1. **Text Preprocessing**
- Lowercasing
- Removing punctuation and digits
- Stopword removal
- Lemmatization using `WordNetLemmatizer`

### 2. **Word Cloud**
- All cleaned text is merged into a single corpus
- Word frequencies are visualized as a cloud using `WordCloud`

### 3. **Topic Modeling (LDA)**
- Use `CountVectorizer` to build a document-term matrix
- Apply `LatentDirichletAllocation` with 3 topics
- Extract top words for each topic

### 4. **Sentiment Analysis**
- Use `TextBlob` to compute polarity scores
- Classify sentiment into: Positive, Negative, Neutral
- Visualize sentiment label distribution using a bar chart

---

## Usage

You can run this notebook in Google Colab or Jupyter:

```python
# Sample usage:
print(df[['doc_id', 'text', 'label']].head())
display_topics(lda, vectorizer.get_feature_names_out(), 5)
```

---

## Results

- Clear sentiment distribution (Positive/Negative/Neutral)
- Word cloud highlights dominant terms
- Topics extracted show common themes from user reviews

---

## Possible Extensions

- Use real-world review datasets (IMDb, Amazon, Twitter)
- Replace `TextBlob` with `VADER`, `Flair`, or `transformers`
- Use `NMF` or `BERTopic` for advanced topic modeling
- Build a Streamlit dashboard for interactive text mining

---

## Author
Project built for the **Text Mining** academic subject. Customize freely for assignments, demos, or presentations!

Feel free to fork and improve 
