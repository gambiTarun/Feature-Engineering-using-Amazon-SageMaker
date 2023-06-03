# Women's Clothing Reviews Sentiment Analysis using BERT and Amazon SageMaker

This project focuses on developing an effective sentiment analysis model based on the Women's Clothing Reviews dataset. It is an end-to-end pipeline using BERT-based natural language processing (NLP) model for classifying customer reviews into positive (1), neutral (0), and negative (-1) sentiments.

## Overview

The project begins by converting the raw review text into machine-readable features suitable for a BERT-based model. This process, known as feature transformation, is executed using an Amazon SageMaker processing job running a custom Python script.

After the feature engineering step, a text classifier model is trained using a variant of BERT known as RoBERTa (Robustly Optimized BERT Pretraining Approach) with the help of a PyTorch model deployed on an Amazon SageMaker Training Job. RoBERTa is a state-of-the-art transformer-based model that improves upon BERT's performance by implementing modifications in its training procedure.

## Key Components

- **Amazon SageMaker Processing Job**: Used for feature transformation, converting the raw review text into machine-readable features, preparing the data for the BERT-based model training.

- **BERT (RoBERTa variant)**: BERT (Bidirectional Encoder Representations from Transformers) is a transformer-based machine learning technique for natural language processing (NLP) pretraining. RoBERTa is a variant of BERT that enhances its performance by optimizing its training process.

- **Amazon SageMaker Training Job**: The PyTorch model leveraging RoBERTa is trained on Amazon SageMaker, a cloud machine learning platform that enables developers and data scientists to build, train, and deploy machine learning models quickly.

By the end of this project, the aim is to have a well-tuned sentiment analysis model capable of classifying customer reviews into positive, neutral, or negative categories with high accuracy.

## Prerequisites
You would need to have an AWS account and knowledge about SageMaker and PyTorch to follow through with this project.

## Data
The dataset used for this project is the Women's Clothing Reviews dataset, which includes a variety of reviews from customers about different clothing items. The dataset has been preprocessed and transformed for use with the BERT-based model.
