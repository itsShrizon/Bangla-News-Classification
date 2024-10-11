**BanglaNewsClassifier: Exploratory Data Analysis**
This document outlines the Exploratory Data Analysis (EDA) performed on the dataset used for the BanglaNewsClassifier project. Our EDA process provides crucial insights into the characteristics of Bangla news articles and informs our subsequent modeling decisions.
Dataset Overview

**Total articles: 118,404**
Categories: 8 (Economic, Technology, Political, Educational, State, International, Sports, Entertainment)
Sources: Various online Bangla news outlets

**Data Distribution**
Category distribution in the dataset:

Economic news: 15.8%
Technology news: 8.4%
Political news: 10.7%
Educational news: 10.8%
State news: 12.8%
International news: 12.9%
Sports news: 14.1%
Entertainment news: 14.3%

Text Characteristics

Average article length: 1,767.52 characters
Minimum length threshold: 50 characters (articles below this were removed)

Preprocessing Steps

HTML tag removal
Punctuation and special character removal
Stop word removal
Stemming using bangla-stemmer library

Word Clouds
We generated word clouds for each category to visualize the most frequent and important terms. These visualizations helped identify key features for classification.
Key Insights

Minor class imbalance observed (7.4% difference between highest and lowest represented categories)
Significant overlap in vocabulary between certain categories (e.g., state and political news)
Distinct terminology identified for categories like sports and technology


