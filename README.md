Depression Detection from Reddit Posts using NLP
📌 Project Overview

Mental health issues such as depression are becoming increasingly common in today's digital world. Many individuals share their emotions, struggles, and personal experiences on social media platforms like Reddit.

However, due to the enormous number of posts generated daily, it is extremely difficult to manually identify users who might be experiencing depression. Early identification of such signals can help provide timely mental health support.

This project focuses on developing an Artificial Intelligence based Natural Language Processing (NLP) system that automatically analyzes Reddit posts and detects whether a post contains signs of depression.

The model reads textual data and classifies posts into two categories:

Depressed

Not Depressed

This automated detection system can assist researchers, mental health professionals, and organizations in understanding emotional patterns expressed on social media.

🎯 Project Objectives

The main objectives of this project are:

To analyze textual data from Reddit posts.

To identify linguistic patterns related to depression.

To build machine learning models capable of detecting depression from text.

To compare different NLP models for classification performance.

To develop an automated system for early detection of depression.

📂 Dataset Description

The dataset used in this project consists of Reddit posts collected from different subreddits.

Depressed Posts (Label = 1)

Posts from communities where users frequently discuss mental health issues, emotional struggles, and depressive feelings.

Examples of such communities include:

r/depression

r/SuicideWatch

Common words found in depressed posts include:

hopeless

worthless

empty

suicidal

burden

darkness

These posts usually express sadness, loneliness, emotional pain, or hopelessness.

Non-Depressed Posts (Label = 0)

Posts collected from general communities where discussions are unrelated to mental health.

Examples include:

r/teenagers

r/Happy

r/DeepThoughts

Common words found in non-depressed posts include:

happy

excited

grateful

fun

gaming

blessed

These posts usually reflect normal daily conversations or positive emotions.

Dataset Statistics

Total number of posts: 831,138

Dataset Split	Number of Posts
Training Data	664,993
Validation Data	83,031
Testing Data	83,114

The dataset is divided into training, validation, and testing sets to ensure proper model training and evaluation.

⚙️ Methodology

The project follows a structured Natural Language Processing pipeline consisting of several stages.

1. Data Collection

Reddit posts were collected from different subreddits related to mental health discussions and general conversations.

2. Text Preprocessing

The raw textual data was cleaned and prepared for machine learning using the following steps:

Converting all text to lowercase

Removing punctuation marks

Removing stopwords

Tokenizing sentences into words

Padding sequences to maintain uniform length

These steps help in improving the quality of input data for model training.

3. Word Representation

Text data cannot be directly used by machine learning models. Therefore, it must be converted into numerical form.

In this project, FastText word embeddings with 300 dimensions were used to convert words into vector representations. FastText helps capture semantic meaning and relationships between words.

4. Model Training

Two deep learning models were implemented to perform depression classification.

BiLSTM (Bidirectional Long Short-Term Memory)

BiLSTM processes the sentence in both forward and backward directions. This allows the model to capture contextual information from both past and future words.

Advantages:

Good at understanding sequential text patterns

Captures contextual relationships between words

BERT (Bidirectional Encoder Representations from Transformers)

BERT is a transformer-based model developed by Google for natural language understanding.

Advantages:

Deep contextual understanding of language

Handles complex linguistic patterns

Achieves higher accuracy for NLP tasks

BERT analyzes the context of each word by looking at both the left and right side of the sentence.

5. Model Evaluation

The trained models were evaluated using the following metrics:

Accuracy – Overall correctness of the model

Precision – Correct positive predictions

Recall – Ability to detect depressed posts

F1 Score – Balance between precision and recall

These metrics help determine how well the model performs in identifying depression-related posts.

🧠 Models Used

The following models were used in this project:

BiLSTM (Bidirectional Long Short-Term Memory)

BERT (Bidirectional Encoder Representations from Transformers)

FastText word embeddings for text representation
