# Emoji Context-Aware Tweets Classification using LSTM and Bi-LSTM

## Project Overview

This project was developed as part of my M.Tech Final Year (Phase-I) project. The objective is to classify tweets into Hate and Non-Hate categories using context-aware deep learning techniques and emoji-enhanced textual representations.

The project uses the Olympics Twitter dataset and incorporates emoji information to improve the understanding of tweet context and sentiment.

## Methodology

### 1. Data Preprocessing
- Dataset cleaning and preprocessing
- Removal of unwanted characters and noise
- Text normalization
- Manual emoji integration and emoji-aware tweet representation

### 2. Feature Extraction

Two feature extraction techniques were implemented:

#### Word Embedding
- GloVe (Global Vectors for Word Representation)

#### N-Grams
- Unigrams
- Bigrams
- Trigrams

Although multiple N-Gram approaches were explored, Bigrams were primarily used in the classification models.

### 3. Deep Learning Models

The following models were developed and evaluated:

- LSTM with GloVe Embeddings
- Bi-LSTM with GloVe Embeddings
- LSTM with Bigrams (Top 10 Features)
- LSTM with Bigrams (Top 5000 Features)
- Bi-LSTM with Bigrams (Top 10 Features)
- Bi-LSTM with Bigrams (Top 5000 Features)

### 4. Clustering and Attention Mechanism

To improve contextual understanding, DBSCAN clustering was integrated with the extracted features and combined with:

- LSTM + Attention Mechanism
- Bi-LSTM + Attention Mechanism

### 5. Evaluation

Model performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## Additional Information

- All implementations were developed using Jupyter Notebook.
- Some ZIP files included in the repository contain datasets and outputs generated during program execution.
- Transfer Learning experiments were also attempted; however, training and execution required significant computational resources and time.

## Technologies Used

- Python
- Jupyter Notebook
- TensorFlow
- Keras
- Scikit-Learn
- GloVe Embeddings
- DBSCAN Clustering
- LSTM
- Bi-LSTM
- Attention Mechanism
- N-Grams

## Dataset

Olympics Twitter Dataset

## Classification Task

Hate Speech Detection

Output Classes:
- Hate
- Non-Hate



## Transfer Learning (Work in Progress)

As an extension of the project, Transfer Learning was explored to improve hate speech classification performance.

Transfer Learning experiments were conducted using a pre-trained hate speech classification dataset. Preliminary implementations were developed to transfer learned knowledge to the Olympics Twitter dataset. Due to training time and hardware limitations, the experiments remain a work in progress and are included as a foundation for future research.
