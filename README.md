# SMS Spam Detection System using NLP and Machine Learning

## Overview
The SMS Spam Detection System is a Natural Language Processing (NLP) and Machine Learning project that classifies SMS messages as **Spam** or **Ham (Normal)**. It uses TF-IDF to convert text messages into numerical features and machine learning algorithms to predict message categories.

The goal is to help identify unwanted messages and demonstrate a practical NLP classification workflow.

## Features
- SMS dataset loading and exploration
- Missing-value and duplicate checking
- Text feature extraction using TF-IDF
- Spam classification using Multinomial Naive Bayes
- Model comparison using Logistic Regression
- Evaluation using accuracy, precision, recall, and F1-score
- Model and vectorizer saving using Joblib
- Prediction on new SMS messages

## Technologies Used
- Python
- Pandas
- Scikit-learn
- Natural Language Processing (NLP)
- TF-IDF
- Multinomial Naive Bayes
- Logistic Regression
- Joblib
- Jupyter Notebook

## Dataset
The project uses the **SMS Spam Collection Dataset** from the UCI Machine Learning Repository.

- Original messages: 5,572
- Messages after duplicate removal: 5,169
- Normal messages (Ham): 4,516
- Spam messages: 653

## Model Performance

| Model | Accuracy | Spam Precision | Spam Recall | Spam F1-score |
|---|---:|---:|---:|---:|
| Multinomial Naive Bayes | 95.26% | 1.00 | 0.63 | 0.77 |
| Logistic Regression | 96.42% | 0.96 | 0.75 | 0.84 |

Logistic Regression achieved the higher test accuracy and spam F1-score in this experiment. Its spam recall was 75%, meaning it detected 75% of the actual spam messages in the test set.

## How It Works
1. Load and explore the SMS dataset.
2. Remove duplicate messages.
3. Split the data into training and testing sets.
4. Convert messages into numerical features using TF-IDF.
5. Train Naive Bayes and Logistic Regression classifiers.
6. Evaluate and compare their performance.
7. Save the selected model and TF-IDF vectorizer.
8. Load the saved files to classify new messages.

## Installation

Install the required libraries:

```bash
pip install pandas scikit-learn joblib jupyter
```

## Run the Project
1. Clone or download this repository.
2. Open the project in Jupyter Notebook.
3. Run the notebook cells in order to prepare the data, train the models, and evaluate the results.
4. Load `spam_model.pkl` and `tfidf_vectorizer.pkl` to make predictions with the saved Logistic Regression model.

## Saved Model Files
- `spam_model.pkl` — trained Logistic Regression classifier.
- `tfidf_vectorizer.pkl` — fitted TF-IDF vectorizer.

**Note:** Keep both files together when using the saved model. If the repository does not include these files, generate them by running the training notebook.

## Future Improvements
- Develop a Streamlit web application.
- Improve spam recall and reduce missed spam messages.
- Test on additional SMS examples and datasets.
- Deploy the application for online use.

## Learning Outcomes
This project provided practical experience in NLP preprocessing concepts, text vectorization, supervised machine learning, model evaluation, algorithm comparison, and model persistence.

## Author
**Gobinath**  
B.Tech Artificial Intelligence and Data Science Student

GitHub: [gobinath0105-lgtm](https://github.com/gobinath0105-lgtm)  
LinkedIn: [Gobinath on LinkedIn](https://linkedin.com/in/gobinath-gobi)
