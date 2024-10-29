# SentimentClassifier

### Overview
This project involves developing a sentiment classifier to categorize comments as pro-vaccination or anti-vaccination. By leveraging machine learning techniques, the classifier aims to assist public health analysis by revealing trends and insights on vaccine sentiment.

### Objectives

* Build a sentiment classifier for vaccine-related comments using machine learning techniques.
* Address uneven annotations in the initial dataset and expand to a larger annotated dataset.
* Improve classifier accuracy, interpretability, and performance through iterative testing.

### Methodology:
1. Data Preprocessing: Managed uneven dataset annotations, applied tokenization, and standardized text inputs.
2. Feature Representation: Utilized CountVectorizer and TfidfVectorizer to represent text data, capturing essential terms and patterns.
3. Model Selection: Implemented multiple classification models, including:
* Logistic Regression
* Multinomial Naive Bayes
* Perceptron
* Multi-Layer Perceptron (MLP) Neural Network.
* Dummy Classifier (baseline for comparison)
4. Performance Evaluation: Assessed models using metrics such as accuracy, cross-validation scores, and classification reports.

### Results
Below are the detailed results of the models, including F1 scores for positive and negative sentiment detection:

| **Vectorizer** | **Model**                    | **Validation** | **Test** | **F1 Score Positive** | **F1 Score Negative** |
|----------------|------------------------------|----------------|----------|-----------------------|-----------------------|
| TFIDF          | Dummy Classifier             | 51.36%        | 49.97%   | 0%                    | 67%                   |
| Count          | Logistic Regression          | 82.78%        | 84.26%   | 84%                   | 84%                   |
| TFIDF          | Logistic Regression          | 84.45%        | 85.23%   | 86%                   | 85%                   |
| TFIDF          | Multinomial Naive Bayes      | 82.68%        | 83.96%   | 84%                   | 84%                   |
| TFIDF          | Perceptron                   | 79.90%        | 80.53%   | 81%                   | 80%                   |
| TFIDF          | MLP Neural Network           | 84.54%        | 85.68%   | 86%                   | 86%                   |

### Future Directions

Potential improvements include expanding the dataset, enhancing feature representation, and refining algorithms to increase model interpretability and accuracy, which would strengthen the tool's utility for public health insights.

