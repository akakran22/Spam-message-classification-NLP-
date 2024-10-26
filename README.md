OVERVIEW
This project involves classifying SMS messages as either Spam or Ham (not spam). The dataset is analyzed and preprocessed using Python, and multiple features are engineered to improve the classification performance.

DATASET
Source: Kaggle
Shape: 5572 messages with 2 columns: label and message.

STEPS
Data Preprocessing:
Converted labels to binary (0: Ham, 1: Spam).
Handled imbalanced data using Oversampling.

Feature Engineering:
Word Count: Counted words in each message.
Currency Symbols: Checked for currency symbols like $, €, etc.
Numbers: Identified messages containing numeric values.

Data Cleaning:
Removed special characters and numbers.
Converted to lowercase.
Tokenized, removed stop words, and lemmatized words.

Model Building:
Created a TF-IDF matrix for message representation.
Trained classifiers: Multinomial Naive Bayes, Decision Tree, Random Forest, and Voting Ensemble.
Evaluated models using the F1-Score.

Results
Best Model: Random Forest with an F1-Score of 0.994.

Visualization
Countplots and distributions show clear differences between Spam and Ham messages based on word count, currency symbols, and numbers.

Insights
Spam messages often include numbers and currency symbols, while Ham messages usually have fewer of these characteristics.


To run this project, you will need the following packages installed:
Python 
pandas
NumPy
matplotlib
seaborn
nltk
scikit-learn

For cloning:
