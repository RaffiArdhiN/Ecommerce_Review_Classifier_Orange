# Sentiment Analysis

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## Overview

The **Sentiment Analysis** project aims to analyze the sentiment (positive, negative, neutral) of textual data using natural language processing (NLP) techniques and machine learning models. This repository also includes an implementation of sentiment classification using **Orange Data Mining**, a visual programming tool for data analysis and machine learning.

---

## Features

- **Text Preprocessing**: Includes tokenization, stopword removal, stemming, and lemmatization.
- **Feature Extraction**: Utilizes techniques like TF-IDF and word embeddings.
- **Machine Learning Models**: Implements algorithms like Naive Bayes, Logistic Regression, Support Vector Machines (SVM), and decision trees.
- **Orange Data Mining Integration**: Provides a pipeline for sentiment classification using Orange workflows.
- **Evaluation Metrics**: Measures accuracy, precision, recall, and F1-score for model performance.
- **Dataset Support**: Works with various datasets, including custom datasets.
- **Modular Design**: Easy to extend and customize.

---

## Installation

### Prerequisites

Ensure you have Python 3.8+ installed. You can download it from [Python.org](https://www.python.org/). Additionally, install Orange Data Mining from [Orange Website](https://orangedatamining.com/).

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/RaffiArdhiN/SentimentAnalysis.git
   cd SentimentAnalysis
2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
3. Install Orange Data Mining:
   ```bash
   pip install orange3
