# Text Classification: Comparative Study of Machine Learning Algorithms

## Project Overview

This project presents a comparative study of four machine learning algorithms for text classification using the SMS Spam Collection dataset.

The main objective is to evaluate and compare the performance of Decision Tree, K-Nearest Neighbours (KNN), Support Vector Machine (SVM), and Naïve Bayes classifiers in identifying spam and legitimate SMS messages.

The project uses Natural Language Processing (NLP) techniques and TF-IDF (Term Frequency–Inverse Document Frequency) for converting text messages into numerical features.

## Problem Statement

Text classification is an important task in Natural Language Processing. Unwanted spam messages can cause security risks, inconvenience, and information overload.

This project investigates how different machine learning algorithms perform when classifying SMS messages into two categories:

- **Ham:** Legitimate or normal SMS messages.
- **Spam:** Unwanted or unsolicited SMS messages.

## Objectives

- Understand and implement text preprocessing techniques.
- Convert text documents into numerical representations using TF-IDF.
- Implement four machine learning classification algorithms.
- Compare classifier performance using standard evaluation metrics.
- Analyse confusion matrices to understand classification errors.
- Conduct a what-if experiment by modifying the SVM regularization parameter.
- Identify the most suitable classifier based on experimental results.

## Dataset

**SMS Spam Collection Dataset**

Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/228/sms+spam+collection)

Dataset information:
- 5,574 labelled SMS messages in the original dataset.
- Two classification categories: Ham and Spam.
- Text-based input data.
- Binary classification problem.

## Technologies and Libraries

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Natural Language Processing (NLP)

## Methodology

### 1. Data Collection
The SMS Spam Collection dataset is downloaded from the UCI Machine Learning Repository.

### 2. Text Preprocessing
The following preprocessing operations are performed:
- Convert text into lowercase.
- Remove URLs and email addresses.
- Remove punctuation and special characters.
- Remove unnecessary whitespace.
- Remove duplicate messages.

### 3. Feature Extraction

TF-IDF is used to transform text messages into numerical feature vectors.

The implementation uses:
- Unigrams and bigrams.
- Maximum of 10,000 features.
- Minimum document frequency of 2.

The TF-IDF vectorizer is fitted only on training data to avoid data leakage.

### 4. Train-Test Split

The dataset is divided into:
- 80% Training data.
- 20% Testing data.

Stratified sampling is used to preserve class distribution.

### 5. Machine Learning Algorithms

Four classification algorithms are implemented:

| Algorithm | Purpose |
|---|---|
| Decision Tree | Classification using decision rules |
| K-Nearest Neighbours | Classification based on nearest data points |
| Support Vector Machine | Classification using an optimal separating boundary |
| Naïve Bayes | Probabilistic text classification |

### 6. Performance Evaluation

The classifiers are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score

### 7. Confusion Matrix Analysis

Confusion matrices are generated to analyse:
- True Positives
- True Negatives
- False Positives
- False Negatives

### 8. What-If Experiment

An additional experiment is conducted by changing the SVM regularization parameter C.

The following values are tested:
- C = 0.1
- C = 1.0
- C = 10.0

The effect of changing C on classification performance is analysed while keeping the dataset, train-test split and TF-IDF features unchanged.

## Project Structure

```text
Text-Classification-Comparative-Study/
│
├── Text_Classification_Comparative_Study.ipynb
│
├── README.md
│
├── classifier_comparison_results.csv
│
└── svm_what_if_results.csv
```

*The CSV files are generated after executing the notebook.*

## How to Run the Project

1. Clone this repository:

```bash
git clone https://github.com/YOUR-USERNAME/Text-Classification-Comparative-Study.git
```

2. Open Google Colab:

https://colab.research.google.com/

3. Upload the `.ipynb` notebook.

4. Select **Runtime → Run all**.

5. The dataset will be downloaded automatically.

6. Execute all cells to generate evaluation metrics, graphs and confusion matrices.

## Experimental Results

The notebook automatically generates a comparative performance table containing Accuracy, Precision, Recall and F1-score for all four algorithms.

It also generates:
- Class distribution graph.
- Model performance comparison graph.
- F1-score comparison graph.
- Confusion matrices.
- SVM parameter comparison graph.

**Note:** Actual experimental results should be added here after executing the notebook. No performance values are pre-filled or fabricated.

## Conclusion

This project provides an experimental comparison of four commonly used machine learning algorithms for binary text classification.

By using the same dataset, preprocessing procedure, TF-IDF representation and evaluation split, the experiment provides a consistent basis for comparing the classifiers.

The final recommendation is determined from the actual experimental results, considering classification metrics and confusion matrix analysis.

## Learning Outcomes

- Understanding Natural Language Processing fundamentals.
- Practical implementation of text preprocessing.
- Working with TF-IDF feature extraction.
- Understanding different machine learning classifiers.
- Evaluating classification models.
- Analysing classification errors.
- Understanding the effect of hyperparameter tuning.

## Author

**Syed Asrar C.**

B.Tech – Computer Science and Engineering (AI & ML)

SRM Institute of Science and Technology

## License

This project is intended for educational and academic purposes.
