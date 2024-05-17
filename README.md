Toxicity Classification Project
#This project involves building machine learning models to classify the toxicity of tweets. The dataset used is a balanced dataset containing tweets labeled as toxic or non-toxic. Various preprocessing steps were applied to the text data, followed by training and evaluating multiple machine learning models.
Table of Contents
DatasetPreprocessing
Model Training and Evaluation
Results
Dependencies
Dataset
The dataset used in this project is stored in FinalBalancedDataset.csv. 
It contains the following columns:
id: Unique identifier for each tweet
Toxicity: Label indicating whether the tweet is toxic (1) or non-toxic (0)
tweet: The tweet text
The dataset contains 56,745 rows.
Preprocessing
Dropping Unnecessary Columns: Removed the 'Unnamed: 0' column which was not useful for analysis.
Text Cleaning:Removed punctuations and digits from the tweet text.Converted text to lowercase.
Stop Words Removal: Used SpaCy to remove common stop words from the text.
Lemmatization: Applied lemmatization to reduce words to their base forms.
Model Training and Evaluation
Feature Extraction
Two types of feature extraction techniques were used:
Bag of Words (CountVectorizer): Extracted word counts.
TF-IDF (TfidfVectorizer): Extracted term frequency-inverse document frequency values.
Models
The following machine learning models were trained and evaluated:
Support Vector Classifier (SVC)
K-Nearest Neighbors (KNeighborsClassifier)
Logistic Regression
Decision Tree Classifier
Random Forest Classifier
Multinomial Naive Bayes
Evaluation Metrics
For each model, the following metrics were calculated on both the training and test sets:
Accuracy
Precision
Recall
F1 Score
Confusion matrices and ROC-AUC curves were plotted for visualizing the performance.
Results
The results of the models are summarized below:
Model Performance on Train and Test Sets 
# Replace with the path to the generated plotsROC-AUC Curves # Replace with the path to the generated ROC curves
Dependencies
The project requires the following Python libraries:
pandasnumpyscikit-learnmatplotlibseabornnltkspacygensim

Download and Place Dataset:
Place FinalBalancedDataset.csv in the project directory.
Run the Preprocessing and Modeling Script:
bashCopy codepython run_classification.py
This will perform preprocessing, train the models, and generate the performance plots.
Review Results:
Review the generated plots in the output directory to compare model performances.
