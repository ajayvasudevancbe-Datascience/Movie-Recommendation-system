# Movie-Recommendation-system

This project focuses on **movie review sentiment classification** using Natural Language Processing. The objective is to classify movie reviews as **positive or negative** and compare how different text representation techniques affect classification performance.

The dataset contains **10,000 movie reviews** with sentiment labels, where `0` represents a negative review and `1` represents a positive review. The data is approximately balanced. 

Two embedding approaches are used. **Word2Vec** generates 300-dimensional word embeddings, which are averaged to represent each review. **Sentence Transformer using `all-MiniLM-L6-v2`** generates contextual sentence-level embeddings. 

These embeddings are then given to two classification models: **Random Forest and Neural Network**. The four combinations are compared based on their training and testing performance. 

The results show that **Sentence Transformer with Neural Network** performs best, achieving approximately **79.07% test accuracy**. Word2Vec with Random Forest achieves 64.10%, Sentence Transformer with Random Forest achieves 72.81%, and Word2Vec with Neural Network achieves 73.31%. 

The main observation is that **contextual Sentence Transformer embeddings perform better than simple Word2Vec averaging** for this sentiment classification task. However, the high training accuracy of the Sentence Transformer-Neural Network model compared with its test accuracy indicates **potential overfitting**. 

Overall, this project provides practical experience with **NLP, text embeddings, Sentence Transformers, machine learning classification, Neural Networks, model comparison, and performance evaluation**.
