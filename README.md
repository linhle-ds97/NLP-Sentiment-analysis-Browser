# NLP-Sentiment-analysis-Browser

Note: This script is uploaded here for the purpose of being used as a reference for sentiment analysis. Therefore, there is no data available in this repository.

A technology company has multiple online products. In order to understand the attitudes of users toward these products, I conducted a sentiment analysis with the data extracted from Google Reviews. The acquired outcome are top common features, top common adjectives for each feature, and average star rating overtime for each feature. The tables are ready for the use of creating dashboard.

The script has the following steps:

1. Extract all English reviews from BigQuery review datasets. The reason is because there are a lot of reviews written in English while the reviewerLanguages are recorded in other languages rather than English.
2. After having the complete English review datasets, we use NLP to process text, then count the word frequency to find the most commonly mentioned nouns/features. Save the complete table in BigQuery. (Temporarily called : 'Main Word' table)
3. Once having the 'Main Word' table, we use it to create the 'Sub Word' table, in which sub-words are top commmonly used adjectives in the reviews containing main words.

After the table with main words and sub-words are completely created, I create a model in Looker and visualize in in the form of dashboard. The PDF file attached is the capture of dashboard for two products analyzed.
