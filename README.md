# Automation-Automated-Customer-Reviews-Using-NLP
Automated Customer Reviews: Product Category Clustering Using NLP

# Project Overview

## This project focuses on automatically clustering products into meaningful categories based on product names, categories, and reviews using advanced Natural Language Processing (NLP) techniques.
## The final output enables better product organization and summarization.

# Technologies Used

- Python
- Pandas, NumPy
- Sentence-BERT (MiniLM-L6-v2)
- HDBSCAN
- KMeans
- Scikit-learn
- UMAP
- NLTK (Text preprocessing)

# Project Workflow

## 1. Text Preprocessing
- Clean product names and categories by removing noise words, numbers, and special characters.
- Apply lemmatization and advanced stopword filtering.

## 2. Text Embedding
- Convert the cleaned text into semantic vectors using Sentence-BERT (MiniLM-L6-v2).

## 3. Initial Clustering (HDBSCAN)
- Apply HDBSCAN to detect dense clusters without requiring the number of clusters in advance.

## 4. Cluster Refinement (BestKFinder)
- Refine the initial clusters using KMeans based on the best Cosine Silhouette Score.

## 5. Visualization
- Use UMAP to reduce embeddings into 2D for cluster visualization.

## 6. Keyword Extraction
- Extract the top keywords from each cluster for better interpretability.

# Final Output

- Final clustered dataset with meaningful meta-categories.
- Each product labeled with a cluster for downstream summarization and recommendation tasks.

Reason: Best balance between cluster quality, semantic richness, and minimal noise.

Visual Results

HDBSCAN Initial Clustering (UMAP Projection)[Insert UMAP image of initial clustering here]

BestKFinder Optimized Clustering (UMAP Projection)[Insert UMAP image of optimized clustering here]

Final Output

A clean dataset containing:

Product Name

Product Category

Cluster Label (optimized)

Supports scalable summarization and downstream analysis.
