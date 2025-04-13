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
### Text Preprocessing
- Removed noise words and cleaned product names and categories.
- Applied lemmatization and advanced stopword filtering.
  
### Embedding Generation
Converted text into dense vector representations using Sentence-BERT (MiniLM-L6-v2).

### Initial Clustering
Used HDBSCAN to create the initial clusters.
Handled noise and small cluster sizes.

### Cluster Refinement
Applied a custom BestKFinder to optimize cluster numbers using Silhouette Score.

### Keyword Extraction
Extracted top keywords from each final cluster for easy summarization.

# Experiments

## Approach

![image](https://github.com/user-attachments/assets/2e49949c-dc82-4412-89f9-0ecd1d28fe38)


## Selected Approach: Product Name + Categories

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
