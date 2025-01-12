# Sentiment Classification Project

![Header Image](header.png)

## Project Description

This project implements a sentiment classification workflow for user reviews from e-commerce platforms. The analysis is conducted entirely using Orange, incorporating preprocessing, multiple machine learning models, and performance evaluation. Below is an overview of the project structure and methodology.

---

## Workflow Overview

The workflow follows these key steps:
1.  **Data Collection**: Extracted reviews from Lazada, Shopee, and Tokopedia.
2.  **Data Preprocessing**: Applied techniques like tokenization, stopword removal, and data cleaning.
3.  **Model Training**: Trained models using machine learning algorithms such as Support Vector Machines (SVM), k-Nearest Neighbors (kNN), Neural Networks, Naive Bayes, Stochastic Gradient Descent (SGD), and AdaBoost.
4.  **Evaluation**: Evaluated models using accuracy, RMSE, and confusion matrices.

---

## Dataset Information

- **Platforms**: Lazada, Shopee, Tokopedia.
- **Dataset Size**: 400 user reviews.
  - **Training Data**: 365 labeled reviews for model training.
  - **Testing Data**: 35 manually scraped reviews for testing.
- **Sentiment Labels**:
  - **Ratings 1–2**: Negative Sentiment
  - **Ratings 4–5**: Positive Sentiment

---

### Preprocessing Details

- **Transformation**:
  - Converted text to lowercase.
  - Removed accents (e.g., é, ñ).
  - Cleaned HTML elements.
  - Removed URLs.
- **Tokenization**:
  - Split text into tokens based on alphanumeric patterns.
- **Stopword Removal**:
  - Removed common stopwords using the provided list (`combined_stop_words.txt`).

---

### Model Training and Performance
![Model Training Workflow](workflow.png)

| **Model**           | **Description**                                                            | **Accuracy** |
|----------------------|----------------------------------------------------------------------------|--------------|
| **SVM**             | Achieved good performance with balanced predictions.                      | 75%          |
| **kNN**             | Tends to overpredict positive sentiment.                                  | 62%          |
| **Neural Network**  | High accuracy but requires longer training times.                         | 81%          |
| **Naive Bayes**     | Fast training with reliable results.                                       | 78%          |
| **SGD**             | Accurate but required significant computational resources during training.| 78%          |
| **AdaBoost**        | Balances performance across metrics; moderately resource-intensive.       | 74%          |

---

## Contributors

- **Raffi Ardhi Naufal**: Data Preprocessing and Tokenization
- **Arya Aydin Margono**: Model Implementation
- **Muhammad Rafie Al Habsyi Setiawan**: Dataset Collection
- **Boy Aditya Rohmaulana**: Evaluation and Documentation

---

## How to Run

1. **Install Orange**:
   - Ensure Orange is installed on your system. You can download it from [Orange's official website](https://orangedatamining.com/).
2. **Open Workflow**:
   - Load the provided `KlasifikasiSentimen.ows` file in Orange.
3. **Data Input**:
   - Use `datatrain.xlsx` for training and `datatest.xlsx` for testing by importing them into the Orange workflow.
4. **View Results**:
   - Analyze the results directly in Orange using the visualization and evaluation widgets.
