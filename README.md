# SemantiQ Similarity

## Introduction
Semantic similarity between sentences is a foundational challenge in Natural Language Processing (NLP). It plays a critical role in applications such as duplicate question detection in online forums, improving machine translation, and identifying redundant web pages. Accurately measuring how closely two sentences align in meaning enables smarter systems that understand language beyond surface-level syntax. The goal of this project is to discover which model architecture best identifies similarity.

## Approach
This problem is tackled using several machine learning models which are given two sentences as input and output a number 0 or 1. Each model leverages **SkipGram word embeddings** to capture contextual meaning from individual words, allowing it to assess deeper semantic relationships between sentences.

### Key Components:
- SkipGram Embeddings: Pre-trained word vectors that encode semantic relationships.
- Neural Network Architecture: Models that were tested include:
  - Feed Forward Network
  - Recurrent Neural Network
  - Encoder Decoder Model
- Training Data: Quora Question Pairs dataset, which contains labeled examples of semantically similar and dissimilar questions.

## Results
The model demonstrates promising performance in identifying semantically similar sentences. Evaluation metrics such as accuracy, precision, and recall show how effectively each architecure captures contextual meaning and distinguishes between sentence pairs.

![Results](/tex/results.png)

## Dataset
- Source: [Quora Question Pairs](https://www.kaggle.com/datasets/quora/question-pairs-dataset)
- Size: ~400,000 question pairs
- Labels: Binary (1 = similar, 0 = not similar)

## References
- Csernai, Kornél. "First Quora Dataset Release: Question Pairs".
- Sun, Xiaofei et al. *Sentence Similarity Based on Contexts*.
- Quora Question Pairs Dataset (Kaggle)
