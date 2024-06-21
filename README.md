# EDA-on-Tweet-Data

# Twitter Data Analysis

This project performs various analyses on a dataset of 10,000 tweets from January 2020. The analyses include sentiment analysis, text preprocessing, clustering, data visualization, and more. The aim is to gain insights into the sentiments and patterns in the tweets. 


## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Dataset](#dataset)
3. [Data Preprocessing](#data-preprocessing)
4. [Sentiment Analysis](#sentiment-analysis)
5. [Clustering](#clustering)
6. [Data Visualization](#data-visualization)
7. [Additional Analyses](#additional-analyses)
8. [Results](#results)


## Prerequisites

Ensure you have the following packages installed in your Python environment:

- `pickle`
- `numpy`
- `string`
- `re`
- `nltk`
- `vaderSentiment`
- `matplotlib`
- `wordcloud`
- `collections`
- `pandas`
- `sklearn`
- `seaborn`
- `plotly`

## Dataset

The dataset consists of 10,000 tweets from January 2020. Ensure you have the dataset file named `10ktweetsjan2020.jsonl` in the appropriate directory. 

## Data Preprocessing

The preprocessing steps include:

1. Loading the data from a JSON Lines file.
2. Extracting the tweet text.
3. Removing punctuation, numbers, and converting text to lowercase.
4. Removing stopwords using the NLTK library.

## Sentiment Analysis

We perform sentiment analysis using the VADER sentiment analyzer. The sentiments are classified into Positive, Negative, and Neutral categories. We then split the data into training and validation sets and apply various classifiers:

- Naive Bayes
- Random Forest
- Support Vector Machine (SVM)

## Clustering

We apply K-Means clustering to the tweet text. The tweets are vectorized using TF-IDF, and PCA is used to visualize the clusters in 2D space.

## Data Visualization

We create various visualizations to explore the data:

1. Sentiment distribution plot.
2. Word clouds for positive and negative sentiments.
3. N-Grams analysis (bi-grams and tri-grams).
4. Time series analysis of tweet activity.
5. Correlation heatmap and pair plots of user attributes.
6. Distribution of verified and geo-enabled users.

## Additional Analyses

We further analyze the tweet metadata, including:

- Grouping tweets by hour and minute.
- Analyzing tweet sources.
- Correlating user attributes with tweet activity.

## Analysis

### Tweet Sources

The analysis determines which applications or platforms were used to post the tweets, such as Twitter for Android or Twitter for iPhone.

### Replied and Quoted Tweets

- **Replied Tweets**: The number of tweets that are replies to other tweets is counted.
- **Quoted Tweets**: The number of tweets that quote other tweets is counted and a list of these tweets is generated.

### User Statistics

- **Twitter User Account Names**: The screen names of Twitter users along with their followers and friends count are listed.
- **Account with Highest Number of Followers**: The Twitter account with the highest number of followers is identified.

### Tweet Statistics

- **Most Liked Tweets**: The tweets with the highest number of likes (favorites) are listed.
- **User Locations**: The locations of Twitter users are identified.

### Sentiment Analysis

- **Segregation of COVID-19 Related Tweets**: Tweets related to COVID-19 are segregated from non-COVID-19 related tweets.
- **Sentiment Analysis**: Sentiment analysis is performed on both COVID-19 related and non-COVID-19 related tweets using VADER sentiment analysis. The sentiment is categorized as positive, negative, or neutral.

### Word Cloud

- **Word Cloud for All Tweets**: A word cloud is generated for all tweets.
- **Word Cloud for Non-COVID-19 Tweets**: A word cloud is generated for tweets not related to COVID-19.

### Additional Analysis

- **Most Tweeted Users**: The users who have tweeted the most are listed.
- **Popular Hashtags**: The most used hashtags are identified and listed.
- **Average Length of Tweets**: The average length of the tweets is calculated.


## Results

The results of the analyses are displayed as plots and tables within the notebook. Key findings include the distribution of sentiments, the most common n-grams, and patterns in tweet activity over time.
The analysis will also produce various outputs such as:

- List of unique applications or platforms used to post tweets.
- Number of replied and quoted tweets.
- User statistics including followers and friends count.
- Most liked tweets.
- User locations.
- Sentiment analysis results.
- Word clouds for tweets.
- Most tweeted users.
- Popular hashtags.
- Average tweet length.










