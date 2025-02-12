# BanglaNewsClassifier: A Hybrid Machine Learning Approach for High-Accuracy News Classification in Low-Resource Bengali Language  

 
    **Status:** This manuscript is currently under review at *PLOS ONE*.  

!!! warning  
    The dataset used in this study was scraped from publicly available Bangla news websites. While the data is intended for academic research, users are advised to respect copyright and usage policies of the original sources. Always seek permission for commercial use or redistribution.  

---  

## Abstract  
**Background:** Bengali (Bangla) is a low-resource language in natural language processing (NLP), with limited datasets and tools for text classification. This study addresses this gap by developing a machine learning/deep learning (ML/DL) framework for automated Bangla news classification.  

**Methods:** We scraped 118,404 Bangla news articles across 8 categories (e.g., politics, sports, entertainment) and applied language-specific preprocessing (e.g., diacritic normalization, stopword removal). A hybrid model combining Long Short-Term Memory (LSTM) networks and Support Vector Machines (SVM) via stacking achieved **94% accuracy**, outperforming standalone models.  

**Results:** The LSTM+SVM approach outperformed traditional classifiers (e.g., SVM alone: 89%) and deep learning models (e.g., CNN: 90.6%) in handling sequential text patterns and class imbalance.  

**Conclusions:** This work demonstrates the efficacy of hybrid ML/DL models for low-resource languages like Bangla. The framework provides a scalable solution for news categorization and contributes to NLP resource development for underrepresented languages.  

---  

## Introduction  
Bengali is the fifth-most spoken language globally but remains underrepresented in NLP research due to limited labeled datasets and language-specific challenges (e.g., complex script, morphological richness). Existing Bangla NLP tools focus on sentiment analysis or machine translation, but few address news classification. This study introduces **BanglaNewsClassifier**, a pipeline for automated categorization of Bangla news articles using a hybrid ML/DL approach.  

---  

## Methods  
1. **Dataset Collection:**  
   - Scraped 118,404 articles from 8 Bangla news portals (e.g., Prothom Alo, bdnews24).  
   - Categories: Politics, Economy, Sports, Entertainment, etc.  

2. **Preprocessing:**  
   - Diacritic normalization, tokenization, and removal of noise (e.g., HTML tags).  
   - Custom stopword list for Bangla.  

3. **Model Architecture:**  
   - **LSTM Layer:** Captured sequential text patterns.  
   - **SVM Stacking:** Improved classification robustness by combining LSTM features with SVM.  

4. **Evaluation:**  
   - Metrics: Accuracy, precision, recall, F1-score.  
   - Baselines: CNN, SVM, Naive Bayes.  

---  

## Results  
- **Best Model (LSTM+SVM):** 94% accuracy, 93.5% F1-score.  
- **Comparison with Baselines:**  
  | Model          | Accuracy | F1-Score |  
  |----------------|----------|----------|  
  | CNN            | 90.6%    | 89.2%    |  
  | SVM            | 89%      | 87.5%    |  
  | LSTM+SVM       | **94%**  | **93.5%**|  

---  

## Discussion  
The hybrid model’s success highlights the synergy between LSTM’s sequential learning and SVM’s decision boundary optimization. This approach addresses Bangla’s morphological complexity and limited labeled data. Future work includes:  
* Testing on multilingual datasets.  
* Incorporating pre-trained transformers (e.g., BanglaBERT).  

---  

## Conclusion  
BanglaNewsClassifier provides a scalable solution for Bangla news classification, advancing NLP for low-resource languages. The hybrid model offers a template for similar tasks in underrepresented languages.  

---  

## References  
: [Bangla-News-Classification GitHub Repository](https://github.com/itsShrizon/Bangla-News-Classification)  
: [Bangla NLP GitHub Topic](https://github.com/topics/bangla-nlp) (includes tools like BanglaBERT)  
: [Deep Learning for Bangla News Classification](https://github.com/SadabShiper/Bangla-News-Article-Classification)  
