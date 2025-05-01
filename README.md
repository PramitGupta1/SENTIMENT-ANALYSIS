# SENTIMENT-ANALYSIS

COMPANY: CODTECH IT SOLUTIONS

NAME: PRAMIT KUMAR GUPTA

INTERN ID: CT04DA412

DOMAIN: DATA ANALYTICS

DURATION: 4 WEEKS

MENTOR: NELA SANTOSH

## Summary

Summary of the IMDB Sentiment Analysis Project
This notebook demonstrates a machine learning pipeline to perform sentiment classification on movie reviews from the IMDB dataset. The goal is to predict whether a given review expresses a positive or negative sentiment using natural language processing (NLP) and supervised learning algorithms.

Libraries and Packages Used
Pandas & NumPy

Used for data manipulation and numerical operations.

pandas is primarily used for reading the dataset, cleaning, and transforming text data.

Matplotlib & Seaborn

These are used for data visualization.

Sentiment distribution is visualized using count plots to better understand the balance between positive and negative reviews.

NLTK (Natural Language Toolkit)

Provides tools for preprocessing text including:

Tokenization using word_tokenize

Removal of stopwords using stopwords.words('english')

Also used for downloading necessary corpora like punkt and stopwords.

WordCloud

Used for creating a visual representation of the most common words in the dataset.

Helps in identifying frequently used terms in reviews.

Scikit-learn

The primary library for machine learning operations:

TfidfVectorizer: Converts text into numerical feature vectors.

train_test_split: Splits the data into training and testing sets.

Models used:

MultinomialNB (Naive Bayes)

LogisticRegression

LinearSVC (Support Vector Classifier)

Evaluation metrics like classification_report and confusion_matrix are used to assess performance.

Regex and String Libraries

Employed to clean text data using pattern matching and character removal.

Project Workflow
1. Loading the Dataset
The dataset is read from a CSV file named "IMDB Dataset.csv", and only the columns review and sentiment are retained. Missing values are removed to ensure clean input for the model.

2. Exploratory Data Analysis (EDA)
A bar chart is created to show the distribution of sentiments (positive vs. negative). A word cloud is also generated to visually inspect the most frequent words in the dataset.

3. Text Preprocessing
A function clean_text is defined that:

Converts all text to lowercase

Removes URLs, mentions, hashtags, and special characters using regular expressions

Tokenizes the text

Removes stopwords and short words (less than 3 characters)

This cleaned text is stored in a new column clean_text.

4. Feature Extraction using TF-IDF
The cleaned text data is vectorized using TfidfVectorizer with a maximum of 3000 features. This step converts textual data into numerical vectors which are used by machine learning models.

5. Train-Test Split
The dataset is split into training and testing sets (most likely 80:20 or similar) to validate model performance on unseen data.

6. Model Training and Evaluation
Three different models are trained on the data:

Naive Bayes: Simple probabilistic model for classification.

Logistic Regression: Linear model effective for binary classification.

Linear SVC: A variation of SVM optimized for linear separation.

Each model is evaluated using classification reports that show precision, recall, F1-score, and overall accuracy, along with confusion matrices for more detailed error analysis.

Expected Output
The final output of this project is:

Performance comparison of different models on the test data.

Visual insights such as sentiment distribution and word clouds.

Cleaned and preprocessed text dataset.

Trained classification models that can predict the sentiment of new movie reviews.

These outputs provide valuable insights into how different ML models perform on a real-world NLP task and establish a framework for further improvements like hyperparameter tuning or using deep learning models.

## Output

![Image](https://github.com/user-attachments/assets/f378c32f-3831-4988-96f4-0675c5d683fb)
![Image](https://github.com/user-attachments/assets/857a4146-8a66-472a-bc20-597c8d438135)
![Image](https://github.com/user-attachments/assets/8f1221d4-e603-4310-a198-206d1f5ca5a4)

