# WELFake News Classification


![1*pfk-nOFPN88EBUxVucokRg](https://github.com/Ceasor06/WELFake-News-Classification/assets/105945382/c464b6ab-39f0-4040-9cbb-d7d3cd327f1c)

## This work presents the solution to one of the kaggle competition that I took part in which is WELFake news classification using Machine Learning methods, Deep Learning and BERT.


(WELFake) is a dataset of 72,134 news articles with 35,028 real and 37,106 fake news. For this, authors merged four popular news datasets (i.e. Kaggle, McIntire, Reuters, BuzzFeed Political) to prevent over-fitting of classifiers and to provide more text data for better ML training.



# Comprehensive Fake News Classification Leveraging LLM

This repository contains the implementation and resources for a project aimed at detecting fake news using traditional machine learning, deep learning, and ensemble learning approaches. The project is built upon the WELFake dataset, which combines multiple benchmark datasets to provide a diverse and extensive source for training and evaluating models.

---

## Project Overview

Fake news detection is a pressing issue in combating misinformation across digital platforms. This project integrates state-of-the-art methodologies, including machine learning algorithms, feature-based classifiers, deep learning architectures, and ensemble models, to achieve high accuracy and robustness in fake news classification.

**Key Features:**
- Utilizes the WELFake dataset comprising over 72,000 news articles.
- Explores multiple machine learning and deep learning approaches, including Logistic Regression, SVM, Random Forest, XGBoost, LSTM, and BERT.
- Implements advanced feature engineering techniques like TF-IDF.
- Employs ensemble learning to combine models and improve performance.

---

## Repository Contents

- **`Data/`**: Directory containing the raw and preprocessed dataset files.
- **`welfake.ipynb`**: Jupyter notebook with the complete project implementation, including data preprocessing, model training, evaluation, and visualization.
- **`preprocessed_dataset.csv`**: Preprocessed dataset used for model training and evaluation.
- **`results/`** *(optional)*: Folder for saving model evaluation metrics, plots, or other output files.

---

## Dataset

The dataset used in this project is the [WELFake Dataset](https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification). It contains:
- **72,134 news articles**:
  - **35,028 real** and **37,106 fake** news.
  - Columns: Serial Number, Title, Text Body, Label (0: Fake, 1: Real).

### Dataset Preview
![Dataset Preview](/Datset_header.png)


---

## Methodology

### 1. **Exploratory Data Analysis (EDA)**
- Analyzed text length, sentiment distribution, word frequency, and n-grams.
- Visualized data using histograms, word clouds, and sentiment polarity graphs.

### 2. **Data Preprocessing**
- Removed null values, URLs, special characters, and stopwords.
- Tokenized, lemmatized, and handled negations.
- Applied TF-IDF for feature engineering.

  Preprocessed Dataset:

![Dataset Preview](/preprocessed_header.png)


### 3. **Modeling**
- **Machine Learning Models**: Logistic Regression, SVM, Random Forest, XGBoost.
- **Deep Learning Models**: LSTM, BERT.
- **Ensemble Models**:
  - Combination of Random Forest, XGBoost, and LSTM.
  - BERT integrated with ensemble models.

### 4. **Evaluation**
- Metrics: Accuracy, Loss.
- BERT and ensemble models achieved the highest accuracy of **99.329%**.

---

## Results

**Best Performing Models:**
- **BERT**: Accuracy - 99.329%, Loss - 0.0531.
- **Ensemble Model 4**: (BERT + Ensemble Model 1) Accuracy - 99.329%, Loss - 0.0423.

**Key Observations:**
- TF-IDF significantly improved the performance of tree-based models.
- Ensemble learning increased robustness and generalization.

*(You can include a plot comparing model performances here.)*

---

## Future Work

- Automate hyperparameter tuning using Optuna.
- Expand to include articles in non-English languages.
- Explore domain-specific datasets in areas like finance, medicine, and law.
- Develop BERT-like models from scratch for greater control over performance.

---

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repository-name.git
