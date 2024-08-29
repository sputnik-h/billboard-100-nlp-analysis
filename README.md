# LyricTrends: NLP Analysis of Billboard Top 100 Songs (1999-2019)

This project conducts a comprehensive analysis of the lyrical content of Billboard Hot 100 songs from 1999 to 2019 using Natural Language Processing (NLP) techniques. The analysis explores the evolution of music and the artists that shaped popular trends through methods such as TF-IDF for trend pivot analysis, LDA for topic modeling, sentiment analysis, and machine learning for popularity prediction.

## Table of Contents
- [Introduction](#introduction)
- [Data Collection and Preparation](#data-collection-and-preparation)
- [Methods](#methods)
- [Results](#results)
- [Conclusion](#conclusion)
- [Limitations](#limitations)
- [Future Work](#future-work)
- [Contributors](#contributors)

## Introduction

The project aims to examine the semantic journey of music lyrics and their impact on song popularity. By analyzing the Billboard Hot 100 songs over two decades, the study focuses on exploring the thematic, sentimental, and genre-specific trends within popular music and develops models to predict song popularity based on lyrical content.

## Data Collection and Preparation

- **Data Source**: The dataset was retrieved from [Kaggle](https://www.kaggle.com/datasets/danield2255/data-on-songs-from-billboard-19992019) and included all songs that entered the Billboard Top 100 from 1999 to 2019, resulting in 7,273 unique songs after cleaning.
- **Preprocessing Steps**:
  - Removed line breaks and lowercased text.
  - Tokenization using regular expressions to extract alphanumeric characters.
  - Removed stopwords using NLTK and a customized list of melodic sounds.
  - Filtered profanities using a reference from YouTube blacklist words.

## Methods

### 1. **TF-IDF Analysis**
   - Performed term frequency (TF) and inverse document frequency (IDF) analysis to identify commonly used and unique words across different time periods and genres.

### 2. **LDA Topic Modeling**
   - Utilized Latent Dirichlet Allocation (LDA) to identify key themes in lyrics, assessing coherence scores to determine the optimal number of topics.
   - Explored genre-specific topics and used BERTopic to improve interpretability by leveraging transformer models.

### 3. **Sentiment Analysis**
   - Applied NLTK’s VADER tool to evaluate sentiment scores of songs, categorizing them into positive, negative, or neutral sentiments and analyzing changes over time.

### 4. **Machine Learning for Popularity Prediction**
   - Developed six machine learning models, including gradient boosting models using XGBoost and TensorFlow/Keras, to predict song popularity based on lyrical features.
   - Created interaction terms between sentiment and genre to enhance prediction accuracy.

## Results

- **TF-IDF Analysis**: Highlighted consistent use of terms like "love," "like," "baby," and "know," underscoring a focus on romantic themes across decades.
- **Topic Modeling**: Identified prominent themes such as romance, wealth, and genre-specific topics like party culture in rap and rural themes in country music.
- **Sentiment Analysis**: Found a dominance of positive sentiment in popular songs, with noticeable declines in positivity in recent years, particularly in genres like Rap and Rock.
- **Popularity Prediction**: Models indicated limited predictive power, highlighting the complexity of popularity factors beyond lyrical content alone.

## Conclusion

The study reveals significant insights into the thematic and sentimental evolution of popular music lyrics, with implications for music producers and streaming services. By identifying lyrical trends and sentiment shifts, the project offers valuable data-driven perspectives on music production and audience engagement.

## Limitations

- The dataset is English-dominant, limiting the generalizability of findings to non-English music.
- Generic stopword lists may retain high-frequency, low-value words that affect the analysis.
- External factors like artist influence, marketing, and cultural impact were not included, which could affect a song’s popularity.

## Future Work

- Incorporate multilingual datasets to broaden the scope of analysis.
- Include external variables like artist influence, marketing campaigns, and media exposure to enhance predictive models.

## Contributors

- Zefeng Lu
- Evelyn Jia
- Angela Zhu
- Nuo Jia
- **Ethan Liu (Machine Learning for Popularity Prediction)**

