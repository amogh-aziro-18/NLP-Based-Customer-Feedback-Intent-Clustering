# NLP-Based-Customer-Feedback-Intent-Clustering

## Project Overview

This project focuses on analyzing unstructured customer feedback to discover underlying intents, patterns, and sentiment trends. Using Natural Language Processing (NLP) and clustering algorithms, we group similar feedback together to help businesses understand customer needs and pain points efficiently.

The pipeline includes:

1. Text preprocessing (cleaning, lemmatization, stopword removal)

2. Sentiment analysis

3. Embedding generation using Sentence-BERT

4. Multiple clustering algorithms (K-Means, DBSCAN, HDBSCAN, Agglomerative, GMM, Spectral, Affinity Propagation)

5. Cluster comparison and evaluation

6. Cluster theme extraction (keywords and sample feedback)

7. Visualization with t-SNE and WordClouds

## Problem Statement

Customer feedback is often unstructured and voluminous, making it hard for businesses to manually detect trends or recurring issues.

The goal is to:

1. Automatically group feedback by intent or theme

2. Detect sentiment polarity for each cluster

3. Provide actionable insights for product, service, and operational improvements

## Pipeline / Methodology

### 1. Data Loading & Cleaning

i. Load CSV dataset

ii. Split combined column into meaningful features (Text, Sentiment, Source, etc.)

iii. Handle missing values and duplicates

### 2. Exploratory Data Analysis (EDA)

i. Inspect dataset structure

ii. Analyze sentiment distribution and text length

iii. Visualize patterns with histograms and charts

### 3. Text Preprocessing

i. Lowercasing and punctuation removal

ii. Stopword removal

iii. Lemmatization

iv. Produces a clean text column ready for embeddings

### 4. Sentiment Analysis

i. Uses VADER to compute sentiment scores

ii. Labels feedback as Positive, Negative, or Neutral

### 5. Feature Extraction

i. Convert text into semantic embeddings using Sentence-BERT

ii. Captures the meaning of text beyond keyword matching

### 6. Clustering

1. Applies multiple clustering algorithms:

i. K-Means

ii. DBSCAN

iii. HDBSCAN

iv. Agglomerative Clustering

v. Gaussian Mixture Model (GMM)

vi. Spectral Clustering

vii. Affinity Propagation

2. Identifies clusters representing customer intents

### 7. Visualization

i. t-SNE plots for cluster separation

ii. Bar charts for cluster size and sentiment distribution

iii. WordClouds for top keywords per cluster

### 8. Cluster Interpretation

i. Extracts top keywords and sample feedback for each cluster

ii. Converts numeric cluster labels into meaningful themes

iii. Helps stakeholders understand feedback intent

### 9. Insights & Recommendations

i. Provides actionable insights based on cluster patterns

ii. Suggests which clustering model captures customer intent most effectively

## Key Features

1. Multi-algorithm clustering pipeline

2. Integrated sentiment analysis

3. Semantic embeddings for better intent capture

4. Comparison of clustering results

5. Cluster theme extraction for interpretability

6. Interactive visualizations

## Technologies Used

1. Python 3.12

2. pandas, numpy – Data manipulation

3. NLTK – Text preprocessing and sentiment analysis

4. Sentence-Transformers – Semantic embeddings

5. scikit-learn – Clustering algorithms

6. hdbscan – Density-based clustering

7. Plotly – Interactive visualizations

8. WordCloud – Cluster theme visualization

## Results

1. Clusters representing feedback intents (e.g., Product Complaints, Positive Experience, Customer Support Issues)

2. Sentiment distribution across clusters

3. Visualizations: t-SNE plots, bar charts, WordClouds

4. Keywords and sample feedback for each cluster

## Insights

1. HDBSCAN or Agglomerative Clustering often provide the most meaningful intent clusters

2. Density-based algorithms can detect small but important customer issues

3. Semantic embeddings outperform keyword-only methods for short feedback
