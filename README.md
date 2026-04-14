# 🎬 Movie Review Sentiment Analyzer — IMDB Dataset

A Natural Language Processing (NLP) project that classifies IMDB movie reviews as **Positive** or **Negative** using machine learning.

---

## 📊 Results

| Model | Accuracy |
|---|---|
| ✅ Logistic Regression | **90.21%** |
| Naive Bayes | 87.94% |

> **Best Model: Logistic Regression with 90.21% accuracy**

---

## 📁 Dataset

- **Source:** [IMDB Dataset of 50K Movie Reviews — Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)
- **Size:** 50,000 reviews — 25,000 Positive + 25,000 Negative
- **Balance:** Perfectly balanced dataset (no class imbalance)

---

## 🛠️ Tech Stack

| Library | Purpose |
|---|---|
| `NLTK` | Tokenization, Stop Word Removal, Stemming |
| `Scikit-learn` | TF-IDF Vectorization, Model Training, Evaluation |
| `Pandas` | Data Loading and Preprocessing |
| `NumPy` | Numerical Operations |
| `Matplotlib` | Charts and Visualizations |
| `Seaborn` | Confusion Matrix and Statistical Plots |

---

## 🔄 Project Pipeline

```
Raw Text Reviews
      ↓
Text Preprocessing (NLTK)
  • Remove HTML tags
  • Tokenization
  • Stop Word Removal
  • Stemming (PorterStemmer)
      ↓
TF-IDF Vectorization (50,000 features, unigrams + bigrams)
      ↓
Model Training
  • Logistic Regression
  • Naive Bayes
      ↓
Evaluation
  • Accuracy, Precision, Recall
  • Confusion Matrix
  • Feature Importance Plot
```

---

## 📌 Key Steps Explained

### 1. Text Preprocessing
- **HTML Tag Removal** — IMDB reviews contain `<br />` tags which are stripped out
- **Tokenization** — Splits sentences into individual words using NLTK
- **Stop Word Removal** — Removes meaningless words like 'the', 'is', 'and'
- **Stemming** — Reduces words to root form: 'loved' → 'love', 'movies' → 'movi'

### 2. TF-IDF Vectorization
Converts cleaned text into numerical features. Words that are important in a specific review but rare across all reviews get a **higher score** — helping the model focus on meaningful words like 'brilliant' or 'terrible'.

### 3. Models
- **Logistic Regression** — Learns word combinations that predict sentiment. Achieved **90.21%** accuracy.
- **Naive Bayes** — Probabilistic model based on word probabilities. Achieved **87.94%** accuracy.

---

## 📈 Visualizations

- ✅ Sentiment Distribution (bar chart)
- ✅ Model Accuracy Comparison
- ✅ Confusion Matrices (both models)
- ✅ Top 20 Most Influential Words (positive & negative)
- ✅ Top 30 Most Frequent Words in Dataset

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/imdb-sentiment-analysis.git
cd imdb-sentiment-analysis
```

### 2. Install dependencies
```bash
pip install nltk scikit-learn pandas numpy matplotlib seaborn
```

### 3. Download the dataset
Download `IMDB Dataset.csv` from [Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews) and place it in the project folder.

### 4. Run the notebook
```bash
jupyter notebook IMDB_Sentiment_Analysis.ipynb
```

---

## 🧪 Test on Custom Reviews

```python
predict_sentiment("This movie was absolutely brilliant! One of the best films I have ever seen.")
# Sentiment: POSITIVE | Confidence: 98.0%

predict_sentiment("Terrible movie. Complete waste of time. The acting was awful and boring.")
# Sentiment: NEGATIVE | Confidence: 100.0%
```

---

## 📂 Project Structure

```
imdb-sentiment-analysis/
├── IMDB_Sentiment_Analysis.ipynb   # Main notebook with all code and outputs
└── README.md                       # Project documentation
```

---

## 👤 Author

**Sai Kumaru Naidu Bandaru**  
[GitHub](https) · [LinkedIn](https://www.linkedin.com/in/bandaru-sai-kumar-naidu/)

