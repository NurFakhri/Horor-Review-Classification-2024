# Classification of Indonesian Horror Movies Reviews in 2024 👻🎥

![image](https://github.com/user-attachments/assets/98754895-5505-4dda-8bd4-e2d361a14372)


## About
This project focuses on building a text classification model to analyze and categorize reviews of Indonesian horror films from 2024. By leveraging natural language processing (NLP) techniques, the project aims to classify reviews into predefined sentiment categories (e.g., positive, negative, or neutral).  

### Key features of the project:  
- **Dataset:** Includes user reviews of Indonesian horror movies released in 2024.  
- **Objective:** Develop a robust classification model to understand audience sentiment and provide insights into movie reception.
- **Applications:** Useful for filmmakers, marketers, and streaming platforms to assess viewer opinions and improve future productions.  

## Dataset

The dataset used in this project consists of tweets from X (formerly known as Twitter) that provide reviews of Indonesian horror films released in 2023. Each tweet has been labeled into one of three sentiment classes:  

1. **Positive:** Tweets expressing favorable opinions, praise, or enthusiasm about the films.  
2. **Negative:** Tweets highlighting dissatisfaction, criticism, or dislike for the films.  
3. **Neutral:** Tweets with impartial or balanced sentiments, providing observations without strong opinions.  

**Dataset Details:**  
- **Source:** Publicly available tweets scraped from X.  
- **Size:** Using 300 out of 10000 with each class of 100 data.  
- **Language:** Bahasa Indonesia.  
- **Features:** Text (the content of the tweet).   

## Depedencies
**Dependencies**  

1. **Core Libraries:**  
   - **`numpy`**: For numerical computations and array manipulations.  
   - **`pandas`**: For data manipulation and analysis, especially handling structured data.  
   - **`matplotlib`**: For creating static, animated, and interactive visualizations.  
   - **`seaborn`**: For advanced and attractive statistical data visualizations.  

2. **Natural Language Processing (NLP) Libraries:**  
   - **`nltk`**: For text processing tasks such as tokenization, stopword removal, stemming, and lemmatization.  
   - **`Sastrawi`**: A library specifically designed for stemming in Bahasa.  
   - **`gensim`**: For building and training word embedding models like FastText and Word2Vec.  

3. **Scikit-learn:**  
   - Provides tools for feature extraction (e.g., `CountVectorizer`, `TfidfVectorizer`), data splitting (`train_test_split`), model building (`DecisionTreeClassifier`), and evaluation (`accuracy_score`, `classification_report`, `confusion_matrix`).  

4. **Other Libraries and Modules:**  
   - **`re`**: For regular expressions, useful in text cleaning and pattern matching.  
   - **`collections.Counter`**: For counting frequency of tokens or n-grams in the text data.  

## Methodology
**Methodology**  

1. **Import Libraries and Load Data**  
   - Import all necessary libraries for data processing, visualization, and model building.  
   - Download required NLTK corpora such as `stopwords`, `wordnet`, and `punkt`.  
   - Load the dataset containing Indonesian horror film reviews from 2023.  

2. **Preprocessing**  
   - **Cleaning:**  
     - Handle slang words by replacing them with their standard forms.  
     - Remove unnecessary symbols, punctuation, and special characters using regular expressions.  
     - Remove numbers to focus only on textual information.  
   - **Stemming:**  
     - Use the Sastrawi library to stem words in Bahasa Indonesia to their root forms.  
   - **Stopword Removal:**  
     - Remove common Bahasa Indonesia stopwords using NLTK or a custom stopword list to reduce noise.  

3. **Training Using Decision Tree Classifier**  
   - Transform the cleaned and preprocessed text into numerical features using different vectorization techniques:  
     - **Bag-of-Words (BoW):** Unigram representation.  
     - **2-grams and 3-grams:** Capture sequential word patterns.  
     - **TF-IDF:** Weight terms by importance and frequency.  
     - **Word2Vec:** Learn distributed word embeddings using Gensim.  
   - Train a Decision Tree classifier for each feature representation.  

4. **Evaluate the Best Model**  
   - Evaluate each model's performance using metrics like accuracy, precision, recall, F1-score, and confusion matrix.  
   - Compare results across different feature representations (BoW, n-grams, TF-IDF, Word2Vec) to determine the best-performing approach.  
   - Visualize the evaluation results for better interpretability and model selection.  

This structured methodology ensures a systematic approach to developing and evaluating the text classification model for Indonesian horror film reviews.

## Result and Insight
