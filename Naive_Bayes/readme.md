# Political Tweet Classifier

This project aims to classify tweets from political candidates as either Republican or Democratic using a Naive Bayes classifier. The dataset includes tweets from both parties, and the classifier is trained to distinguish between them based on the textual content of the tweets.

## Dataset

The dataset is stored in a SQLite database named `congressional_data.db`, which contains two tables:
- `candidate_data`: Information about political candidates, including their party affiliation.
- `tweets`: Tweets posted by the candidates.

## Preprocessing

The preprocessing steps include:
1. Extracting tweets and their corresponding party affiliations from the database.
2. Cleaning and tokenizing the tweet text.
3. Creating a balanced dataset by sampling an equal number of tweets from each party.
4. Converting the tweets into feature vectors using words that occur more than a specified number of times (word cutoff).

## Feature Extraction

Features are extracted from the tweets using the following steps:
1. Clean and tokenize the text.
2. Create a set of feature words based on their frequency in the dataset.
3. Convert each tweet into a feature vector indicating the presence or absence of each feature word.

## Model Training

A Naive Bayes classifier is trained on the feature vectors to classify the tweets as either Republican or Democratic. The model is evaluated using accuracy and a confusion matrix.

## Results

The classifier achieves an accuracy of 61.40%. The confusion matrix shows the number of correctly and incorrectly classified tweets for each party.

### Confusion Matrix

| Actual \ Estimated | Republican | Democratic |
|--------------------|------------|------------|
| Republican         | 1662       | 2699       |
| Democratic         | 799        | 4842       |

## Reflections

The classifier shows moderate accuracy but has difficulty accurately distinguishing between tweets from Republican and Democratic candidates. The model tends to misclassify Republican tweets as Democratic more frequently. Enhancements in feature engineering and using more advanced models could improve performance.
