🎬 Movie Review Sentiment Analyzer — IMDB Dataset
A Natural Language Processing (NLP) project that classifies IMDB movie reviews as Positive or Negative using machine learning.


📊 Results
ModelAccuracy✅ Logistic Regression90.21%Naive Bayes87.94%

Best Model: Logistic Regression with 90.21% accuracy


📁 Dataset
1.Source: IMDB Dataset of 50K Movie Reviews — Kaggle
2.Size: 50,000 reviews — 25,000 Positive + 25,000 Negative
3.Balance: Perfectly balanced dataset (no class imbalance)

🛠️ Tech Stack
Library         Purpose
NLTK            Tokenization, Stop Word Removal, Stemming
Scikit-learn    TF-IDF Vectorization, Model Training, Evaluation
Pandas          Data Loading and Preprocessing
NumPy           Numerical Operations
Matplotlib      Charts and Visualizations
Seaborn         Confusion Matrix and Statistical Plots

🔄 Project Pipeline
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

  📌 Key Steps Explained
  
1. Text Preprocessing
     HTML Tag Removal — IMDB reviews contain <br /> tags which are stripped out
     Tokenization — Splits sentences into individual words using NLTK
     Stop Word Removal — Removes meaningless words like 'the', 'is', 'and'
     Stemming — Reduces words to root form: 'loved' → 'love', 'movies' → 'movi'
   
2. TF-IDF Vectorization
     Converts cleaned text into numerical features.
     Words that are important in a specific review but rare
     across all reviews get a higher score — helping
     the model focus on meaningful words like'brilliant' or 'terrible'

3. Models
     Logistic Regression — Learns word combinations that predict sentiment. Achieved 90.21% accuracy.
     Naive Bayes — Probabilistic model based on word probabilities. Achieved 87.94% accuracy.


📈 Visualizations

✅ Sentiment Distribution (bar chart)
✅ Model Accuracy Comparison
✅ Confusion Matrices (both models)
✅ Top 20 Most Influential Words (positive & negative)
✅ Top 30 Most Frequent Words in Dataset


🚀 How to Run
1. Clone the repository

  git clone https://github.com/YOUR_USERNAME/imdb-sentiment-analysis.git
  cd imdb-sentiment-analysis

2. Install dependencies

 pip install nltk scikit-learn pandas numpy matplotlib seaborn

3. Download the dataset
 Download IMDB Dataset.csv from Kaggle and place it in the project folder.

4. Run the notebook
   
     
