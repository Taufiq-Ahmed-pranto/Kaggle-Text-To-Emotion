# Natural Language Processing & Text Mining Project

## Project Overview

The goal of this project is to explore and analyze the Kaggle Text to Emotion Dataset, specifically the [Emotion Detection from Text dataset](https://www.kaggle.com/datasets/pashupatigupta/emotion-detection-from-text/data?select=tweet_emotions.csv). The dataset contains 40,000 Twitter records classified into 13 emotion categories.

### Initial Exploration

1. **Histogram of Categories**
   - Write a script inspired by existing Kaggle programs to output the histogram of the different emotion categories.
   - Comment on the distribution of training samples across various categories.

2. **Concatenation and Keyword Analysis**
   - Concatenate all tweets of the same category into a single file (data frame).
   - Output the top 10 most frequent keywords in each category before and after processing (e.g., stopword removal, unusual character removal).

3. **Token Analysis and WordCloud**
   - Write a script to output the histogram of the 10 most frequent tokens in each category (data frame).
   - Generate WordClouds for each data frame.

### Category Reduction

4. **Manual Crafting (Construction A)**
   - Suggest a manual crafting method assigning each category to Positive, Negative, or Neutral.
   - Present a table mapping the 13 categories to the constructed Positive, Negative, and Neutral categories.

5. **Word2Vec Embedding (Construction B)**
   - Use k-means clustering with k=3 on the 13 Word2Vec embedding vectors of category titles.
   - Summarize the content of each class in terms of the 13 categories.
   - Present a table mapping the 13 categories to the constructed Positive, Negative, and Neutral categories.

### Evaluation Metrics

6. **Overlap Analysis**
   - Write a script to compute the total number of common tokens in each class for both constructions A and B.
   - Provide a summary table synthesizing the number of common tokens for each class in A and B.

7. **Frequent Word Analysis**
   - Repeat the analysis considering the sets of 20 most frequent words for each data frame.
   - Summarize the result in a table for both constructions A and B.

8. **Wordnet Lexical Database Analysis**
   - Write a script to check if a term has an entry in WordNet lexical database.
   - Output the number of unmatched tokens and the corresponding percentage in each data frame.
   - Summarize the result in a concise table.

### Stylometric Features and NRC Lexicon

9. **NRC Word-Emotion Association Lexicon**
   - Calculate the entity value for each record and category using the NRC Lexicon.
   - Construct vectors V1 (labeling vector) and V2 (NRC-based vector) for each category.
   - Use Pearson correlation coefficient to analyze the correlation between V1 and V2 for each category.
   - Present the results in a table with correlation values and p-values.

### Category Similarity

10. **Title vs. Record-Based Similarity**
    - Write a function to calculate similarity between records in two categories using word2vec embedding.
    - Generate a matrix of record-based similarity between each pair of categories.
    - Discuss the matching outcome between title similarity and record-based similarity.

11. **Extended Analysis with Different Embeddings**
    - Repeat 10) using Glove, FastText, and BERT (base) embeddings.
    - Discuss any variations in the matching outcome.

12. **State-of-the-Art Approach**
    - Suggest an extra state-of-the-art approach for matching category content to category title.
    - Identify appropriate literature to comment on the findings.
