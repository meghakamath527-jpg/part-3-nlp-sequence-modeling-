## NLP and Sequence Modeling Mini Project
# Task 1: Dataset Understanding
# Number of Records

The dataset contains multiple text records used for NLP classification.

# Target Labels/Classes

The dataset contains different target categories represented using labels.

# Sample Text Records

Sample text records were displayed to understand sentence structure and content patterns.

# Average Text Length

Average text length was calculated to understand sequence size and padding requirements.

# Class Distribution

Class distribution was visualized using count plots to identify dataset balance.

## Task 2: Text Preprocessing

The following preprocessing steps were applied:

# Lowercasing

All text was converted into lowercase to maintain consistency.

# Removing Special Characters

Symbols and unnecessary punctuation were removed using regular expressions.

# Tokenization

Sentences were split into individual words/tokens.

# Stopword Removal

Common words such as:

the
is
and
of

were removed because they do not contribute much semantic meaning.

# Padding and Truncation

Sequences were padded or truncated to maintain equal sequence length for LSTM input.

## Task 3: Text Vectorization
# TF-IDF Vectorization

Text was converted into numerical vectors using TF-IDF.

TF-IDF gives importance to words that are:

* frequent in one document
* but rare across all documents

This helps improve text classification performance.

# Why Text Must Be Converted Into Vectors

Machine learning models cannot understand raw text directly.

Text must be converted into numerical format because:

* models perform mathematical computations
* vectors represent text numerically
* neural networks require numerical input tensors
## Task 4: Baseline Model
# Model Used

Logistic Regression with TF-IDF features was used as the baseline model.

# Evaluation Metrics

The model was evaluated using:

* Accuracy
* Classification Report
* Confusion Matrix

The baseline model successfully classified text records into their respective categories.

## Task 5: Sequence Model
# LSTM Architecture

The sequence model contains:

# Input Sequence

Text is converted into token sequences.

# Embedding Layer

The embedding layer converts tokens into dense vector representations.

# LSTM Layer

The LSTM learns sequential dependencies and contextual relationships between words.

# Dense Layer

Fully connected layers perform classification using learned sequence features.

# Output Layer

The output layer predicts final class probabilities.

# Loss Function

Binary crossentropy was used for binary classification tasks.

# Evaluation Metric

Accuracy was used to measure model performance.

## Task 6: Attention and Transformer Reflection
# Why RNNs Struggle with Long-Term Dependencies

Traditional RNNs struggle to remember earlier information in long sequences due to the vanishing gradient problem.

# How LSTMs Help with Memory

LSTMs use memory cells and gating mechanisms to preserve important information for longer durations.

# What Attention Solves

Attention helps the model focus on important words in the input sequence rather than compressing everything into a single hidden state.

This improves performance in:

* translation
* summarization
* text generation
# Why Transformers are Important

Transformers process text in parallel and use self-attention mechanisms.

Advantages:

* Faster training
* Better context understanding
* Improved scalability
* Foundation of modern Generative AI models like GPT and BERT
