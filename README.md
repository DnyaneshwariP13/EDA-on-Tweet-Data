# EDA-on-Tweet-Data

# Twitter Data Analysis

This project performs various analyses on a dataset of 10,000 tweets from January 2020. The analyses include sentiment analysis, text preprocessing, clustering, data visualization, and more. The aim is to gain insights into the sentiments and patterns in the tweets.

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Installation](#installation)
3. [Dataset](#dataset)
4. [Data Preprocessing](#data-preprocessing)
5. [Sentiment Analysis](#sentiment-analysis)
6. [Clustering](#clustering)
7. [Data Visualization](#data-visualization)
8. [Additional Analyses](#additional-analyses)
9. [Results](#results)
10. [Contributing](#contributing)
11. [License](#license)

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

## Installation

Clone this repository and navigate to the project directory:

```bash
git clone https://github.com/yourusername/twitter-data-analysis.git
cd twitter-data-analysis
```

Install the required packages:

```bash
pip install -r requirements.txt
```

## Dataset

The dataset consists of 10,000 tweets from January 2020. Ensure you have the dataset file named `10ktweetsjan2020.jsonl` in the appropriate directory. The file should contain tweets with the following structure:

```json
{
  "full_text": "Your tweet text here",
  ...
}
```

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

## Results

The results of the analyses are displayed as plots and tables within the notebook. Key findings include the distribution of sentiments, the most common n-grams, and patterns in tweet activity over time.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

Feel free to customize the README further to better suit your project. This template provides a comprehensive overview of the analyses performed and instructions for running the project.
