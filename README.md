

Toxicity Classification Project
This project involves building machine learning models to classify the toxicity of tweets. Let’s dive into the specifics:

Dataset
The dataset contains 56,745 rows.
Columns:
id: Unique identifier for each tweet.
Toxicity: Label indicating whether the tweet is toxic (1) or non-toxic (0).
tweet: The tweet text.
Preprocessing
Dropping Unnecessary Columns:
Removed the ‘Unnamed: 0’ column, which was not useful for analysis.
Text Cleaning:
Removed punctuation and digits from the tweet text.
Converted text to lowercase.
Stop Words Removal:
Used SpaCy to remove common stop words from the text.
Lemmatization:
Applied lemmatization to reduce words to their base forms.
Feature Extraction
Two techniques used:
Bag of Words (CountVectorizer): Extracted word counts.
TF-IDF (TfidfVectorizer): Extracted term frequency-inverse document frequency values.
Models
Trained and evaluated various machine learning models:

Support Vector Classifier (SVC)
K-Nearest Neighbors
Logistic Regression
Decision Tree Classifier
Random Forest Classifier
Multinomial Naive Bayes
Evaluation Metrics
For each model, calculated metrics on both training and test sets:

Accuracy
Precision
Recall
F1 Score
Visualized performance using confusion matrices and ROC-AUC curves.

Dependencies
The project requires the following Python libraries:

pandas
numpy
scikit-learn
matplotlib
seaborn
nltk
spacy
gensim
bashCopy codepython run_classification.py
This will perform preprocessing, train the models, and generate the performance plots.
Review Results:
Review the generated plots in the output directory to compare model performances.
