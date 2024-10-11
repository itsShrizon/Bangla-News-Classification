# BanglaNewsClassifier: Exploratory Data Analysis

This document outlines the Exploratory Data Analysis (EDA) performed on the dataset for the **BanglaNewsClassifier** project. Our EDA process provides crucial insights into the characteristics of Bangla news articles and informs subsequent modeling decisions.

---

## Dataset Overview

- **Total Articles**: 118,404
- **Categories**: 8 
  - Economic
  - Technology
  - Political
  - Educational
  - State
  - International
  - Sports
  - Entertainment
- **Sources**: Various online Bangla news outlets

---

## Data Distribution

Category distribution within the dataset:

- **Economic news**: 15.8%
- **Technology news**: 8.4%
- **Political news**: 10.7%
- **Educational news**: 10.8%
- **State news**: 12.8%
- **International news**: 12.9%
- **Sports news**: 14.1%
- **Entertainment news**: 14.3%

---

## Text Characteristics

- **Average article length**: 1,767.52 characters
- **Minimum length threshold**: 50 characters (articles below this were removed)

---

## Preprocessing Steps

1. **HTML tag removal**
2. **Punctuation and special character removal**
3. **Stop word removal**
4. **Stemming**: Utilized the `bangla-stemmer` library

---

## Word Clouds

Word clouds were generated for each category to visualize the most frequent and important terms. These visualizations helped identify key features for classification.

---

## Key Insights

- **Class imbalance**: Minor imbalance observed with a 7.4% difference between the highest and lowest represented categories.
- **Vocabulary overlap**: Significant overlap found between certain categories, especially between *State* and *Political* news.
- **Distinct terminology**: Clear distinct terms identified for categories like *Sports* and *Technology*.

---

### Conclusion

This EDA provided us with valuable insights into the dataset's structure, helping guide feature selection and classification strategies for the **BanglaNewsClassifier** project.
