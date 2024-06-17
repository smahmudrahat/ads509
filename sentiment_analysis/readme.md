# ADS 509 Sentiment Assignment

This project holds the Sentiment Assignment for Module 6 in ADS 509, Applied Text Mining. The goal is to apply sentiment analysis to a dataset of tweets and lyrics from two artists: Cher and Robyn. This README file provides an overview of the steps taken in the project, including data preprocessing, sentiment analysis, and results.

## Dataset

The dataset includes Twitter data and lyrics data for two artists, Cher and Robyn. The dataset is stored in a structured format as follows:

- **Twitter Data:** Contains descriptions posted by followers of the artists.
- **Lyrics Data:** Contains song lyrics for the artists.

## Preprocessing

### Steps:

1. **Extract Data:**
    - Extract tweets and their corresponding party affiliations from the database.
    - Extract lyrics data from the provided files.

2. **Clean and Tokenize:**
    - Clean and tokenize the text from tweets and lyrics.

3. **Create Balanced Dataset:**
    - Sample an equal number of tweets from each party to create a balanced dataset.

4. **Feature Extraction:**
    - Convert the tweets and lyrics into feature vectors using words that occur more than a specified number of times (word cutoff).

## Sentiment Analysis on Songs

### Read in the Lyrics Data

- Extract lyrics data for each artist.
- Convert the nested dictionary of lyrics data into a DataFrame for easier handling.

### Read in the Twitter Data

- Extract Twitter descriptions for each artist.
- Convert the list of Twitter descriptions into a DataFrame.

### Sentiment Calculation

#### Read Positive and Negative Words

- Read positive and negative words from provided files.
- Combine all sentiment words into a single dictionary.

#### Calculate Sentiment Scores

- Define a sentiment calculation function.
- Apply the sentiment calculation function to the lyrics and Twitter descriptions.
- Calculate average sentiment scores for each artist.

### Results

#### Highest Sentiment Songs for Robyn:

- **"Love Is Free"**: Sentiment Score 116
- **"We Dance To The Beat"**: Sentiment Score 66
- **"We Dance To The Beat"**: Sentiment Score 66

#### Lowest Sentiment Songs for Robyn:

- **"Don't Fucking Tell Me What To Do"**: Sentiment Score -93
- **"Don't Fucking Tell Me What To Do"**: Sentiment Score -93
- **"Criminal Intent"**: Sentiment Score -53

The sentiment scores of Robyn's songs are driven by the frequency and type of words used in the lyrics. "Love Is Free" has the highest sentiment score due to its repetitive use of positive words like "free," "love," and "baby," creating an overall positive and carefree theme. Conversely, "Don't Fucking Tell Me What To Do" has the lowest sentiment score, driven by its repetitive use of negative phrases emphasizing frustration and negativity.

#### Highest Sentiment Songs for Cher:

- **"Love And Understanding"**: Sentiment Score 56
- **"I Found You Love"**: Sentiment Score 52
- **"Perfection"**: Sentiment Score 43

#### Lowest Sentiment Songs for Cher:

- **"Bang-Bang"**: Sentiment Score -70
- **"Outrageous"**: Sentiment Score -26
- **"I Walk On Guilded Splinters"**: Sentiment Score -24

Cher's highest sentiment songs emphasize positive themes of love and understanding, with frequent use of uplifting words. In contrast, the lowest sentiment songs focus on negative themes, such as emotional pain and defiance.

## Twitter Sentiment Analysis

### Average Sentiment of Tweets

- **Cher's Followers**: Average Sentiment 0.3528
- **Robyn's Followers**: Average Sentiment 0.2885

### Most Popular Emojis

#### Cher's Followers:
- **Most Popular Positive Emoji**: 😍 (Count: 8955)
- **Most Popular Negative Emoji**: 😭 (Count: 823)

#### Robyn's Followers:
- **Most Popular Positive Emoji**: 😎 (Count: 325)
- **Most Popular Negative Emoji**: 😭 (Count: 42)

The average sentiment of tweets and the most popular emojis reflect the general sentiment of the followers of each artist. Cher's followers tend to use more positive emojis, whereas Robyn's followers also show a predominance of positive sentiment, though slightly less than Cher's followers.

## Reflection

The sentiment analysis shows that Cher's songs and followers generally exhibit a higher average sentiment compared to Robyn's. The analysis highlights the impact of word choice and themes on sentiment scores. Future improvements could include more advanced sentiment analysis techniques and exploring additional features for better classification.

## Conclusion

This project provides insights into the sentiment expressed in the lyrics and Twitter descriptions of two popular artists. By applying text mining and sentiment analysis techniques, we can better understand the emotional tone of their content and their audience's reactions.
