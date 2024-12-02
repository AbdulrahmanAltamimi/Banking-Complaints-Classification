# Banking-Complaints-Classification

This project aims to classify consumer complaints in the banking sector using natural language processing (NLP) techniques. The approach combines Word2Vec embeddings with a VotingClassifier ensemble to improve the accuracy and robustness of the classification.

## Dataset

The dataset used in this project is sourced from [Kaggle: Consumer Complaints Dataset for NLP](https://www.kaggle.com/datasets/shashwatwork/consume-complaints-dataset-fo-nlp). It consists of consumer complaints about financial products and services, including their textual descriptions. The dataset serves as an excellent resource for exploring NLP applications in customer service and issue classification.

### Key Features of the Dataset

- **Text:** Detailed descriptions of consumer complaints.
- **Labels:** Categories representing the type of complaint or product/service involved.

## Approach

### 1. Text Preprocessing
- Tokenization, lemmatization, and removal of stop words.
- Creation of word embeddings using Word2Vec to convert textual data into numerical vectors.

### 2. Classification Model
- Utilizes a `VotingClassifier`, which combines multiple machine learning models (Random Forest, Multilayer Perceptron and SVM) to make ensemble predictions.
- Word2Vec embeddings are used as input features for the models in the VotingClassifier.

### 3. Evaluation
- The model's performance is assessed using metrics such as accuracy, and F1-score.
