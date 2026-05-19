# Part 3 — NLP and Sequence Modeling Mini Project

## Project Overview

This project focuses on Natural Language Processing (NLP) and sequence modeling using customer support text data.

The objective is to understand:
- text preprocessing
- text vectorization
- baseline NLP models
- sequence modeling with LSTMs
- attention and transformers

The project classifies customer messages into sentiment categories.

---

# Dataset Information

Dataset:
- `customer_support_text_classification.csv`

Target Column:
- `sentiment_label`

Classes:
- positive
- neutral
- negative

Useful Columns:
- customer_message
- channel
- word_count
- urgent_flag

---

# Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- TensorFlow / Keras
- Matplotlib
- Seaborn

---

# Project Workflow

1. Dataset understanding
2. Text preprocessing
3. Text vectorization
4. Baseline NLP model
5. Sequence modeling with LSTM
6. Model evaluation
7. Transformer reflection

---

# Text Preprocessing

The following preprocessing steps were applied:

- lowercasing
- removing special characters
- tokenization
- stopword removal
- sequence padding

---

# Text Vectorization

TF-IDF vectorization was used for the baseline model.

Why vectorization is needed:
- machine learning models cannot understand raw text
- text must be converted into numerical vectors

---

# Baseline Model

Model Used:
- Logistic Regression with TF-IDF

Evaluation Metrics:
- Accuracy
- Confusion Matrix
- Classification Report

---

# Sequence Model

Sequence Model Used:
- LSTM

Architecture:
- Input sequence
- Embedding layer
- LSTM layer
- Dense layer
- Output layer

Loss Function:
- sparse_categorical_crossentropy

Evaluation Metric:
- accuracy

---

# Attention and Transformers

## Why RNNs Struggle

RNNs struggle with long-term dependencies because earlier information may fade during sequence processing.

## How LSTMs Help

LSTMs use memory cells and gates to preserve useful information over longer sequences.

## What Attention Solves

Attention helps models focus on important words in a sequence.

## Why Transformers Matter

Transformers use self-attention and parallel processing to improve NLP performance.

Modern Generative AI systems such as ChatGPT are based on transformer architectures.

---

# Repository Structure

```text
part-3-nlp-sequence-modeling/
│
├── README.md
├── notebook.ipynb
├── requirements.txt
├── customer_support_text_classification.csv
│
└── results/
    ├── model_evaluation.csv
    └── sample_predictions.txt
```

---

# Conclusion

This project demonstrated:
- text preprocessing
- vectorization
- sentiment classification
- sequence modeling
- transformer concepts

The project showed how NLP pipelines convert text into meaningful numerical representations for machine learning and deep learning systems.