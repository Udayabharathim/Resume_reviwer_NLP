# Resume_reviwer_NLP

## 1. What is Resume Prediction?
Resume prediction is the process of automatically identifying the job category or career domain (like HR, Data Science, Web Developer) based on the text content of a resume using machine learning.

## 2. Dataset Used
The model uses a dataset of resumes.

Each resume is labeled with a job category.

Only two columns are used: Category (label) and Resume (text).

## 3. Text Preprocessing
Before training, resumes are cleaned using NLP techniques:

Lowercasing: Converts all text to lowercase.

Tokenization: Splits text into individual words.

Stopword Removal: Removes common words like "is", "and", "the".

Lemmatization: Converts words to their base form (e.g., "running" → "run").

This helps simplify the text and reduce noise.

## 4. Feature Extraction (TF-IDF)
TF-IDF (Term Frequency - Inverse Document Frequency) converts text into numerical vectors.

It highlights important words in each resume.

Only the top 5000 features are selected for training.

## 5. Model Training
A Logistic Regression model is used for classification.

The dataset is split into training (80%) and testing (20%) sets.

The model learns from the training data to classify resumes into job categories.

## 6. Sample Output
<img width="307" height="96" alt="image" src="https://github.com/user-attachments/assets/1f374887-ad7c-4a80-a470-c8f4bbcc293e" />


## 7. Model Evaluation
Accuracy is calculated on the test set.

A classification report is printed to show performance for each job category.

## 8. Predicting a New Resume
The user can paste their own resume text.

It is cleaned and transformed like the training data.

The model predicts the most likely job category.
