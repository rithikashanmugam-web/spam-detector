# Spam Message Detection using Machine Learning

## Project Title
Spam Message Detection using Machine Learning and Natural Language Processing

## Objective

The objective of this project is to build a Machine Learning model that can automatically classify SMS/text messages into:

- **Spam** → promotional messages, scams, advertisements, unwanted messages
- **Ham** → genuine personal or normal messages

This project helps automate spam filtering and demonstrates how Machine Learning and NLP can be used in real-world communication systems.


## Problem Statement

Nowadays users receive many unwanted messages such as:

- Lottery messages
- Fake offers
- Promotional advertisements
- Fraud links

Manually filtering all messages is difficult.

This project develops an intelligent spam detection system that reads a message, processes the text, and predicts whether it is **Spam** or **Ham**.

## Dataset Used

Dataset source:

Kaggle – SMS Spam Collection Dataset

https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset

### Dataset details

The dataset contains thousands of SMS messages.

Main columns:

| Column | Description |
|-------|-------------|
| v1 | Label (spam / ham) |
| v2 | SMS message text |

Example:

| Label | Message |
|------|---------|
| ham | Hey are you coming today? |
| spam | Congratulations! You won ₹5000 |

## Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- NLTK
- Scikit-Learn
- Joblib

### Tools
- VS Code
- GitHub
- Kaggle


## Machine Learning Algorithm Used

### Multinomial Naive Bayes

Multinomial Naive Bayes is commonly used for text classification.

Reasons for choosing:

- Fast training
- Works well with text
- High accuracy
- Easy to explain
- Suitable for TF-IDF vectors


## NLP / Text Preprocessing Steps

Before training, raw text is cleaned.

### 1. Convert to lowercase

Example:

HELLO → hello


### 2. Remove punctuation

Example:

Congratulations!!! → Congratulations

### 3. Remove numbers and symbols

Example:

₹5000 → removed


### 4. Remove stop words

Words like:

- the
- is
- and
- are

These words do not add much meaning.


### 5. Tokenization

Sentence is split into words.

Example:

"claim your prize now"

becomes

- claim
- your
- prize
- now


## Feature Extraction

### TF-IDF Vectorizer

Machine Learning cannot understand plain text.

TF-IDF converts text into numbers.

Example:

"free entry"

becomes vector values.

Benefits:

- Measures word importance
- Improves text classification
- Works well with Naive Bayes


## Project Workflow

### Step 1
Download dataset from Kaggle

### Step 2
Load dataset using pandas

### Step 3
Preprocess text

### Step 4
Split data into training and testing

### Step 5
Convert text using TF-IDF

### Step 6
Train Naive Bayes model

### Step 7
Evaluate accuracy

### Step 8
Save trained model

### Step 9
Predict user-entered messages


## Folder Structure

```bash
Spam Message Detection
│
├── data
│   └── spam.csv
│
├── model
│   ├── spam_model.pkl
│   └── vectorizer.pkl
│
├── src
│   ├── preprocess.py
│   ├── train.py
│   └── predict.py
│
├── README.md
├── requirements.txt


## Files Description

### preprocess.py

Responsible for:

- text cleaning
- lowercase conversion
- removing punctuation
- removing stop words


### train.py

Responsible for:

- loading dataset
- preprocessing text
- TF-IDF conversion
- model training
- testing
- saving trained model


### predict.py

Responsible for:

- loading trained model
- taking user input
- predicting spam or ham


## Model Evaluation

Model accuracy achieved:

### Accuracy = 96.68%

Classification report includes:

- Precision
- Recall
- F1-score

Example:

| Label | Precision |
|------|-----------|
| Ham | High |
| Spam | High |


## Sample Prediction

### Input
Congratulations! You won ₹5000 cash prize.

### Output
Spam


### Input
Where are you? Shall we meet today?

### Output
Ham


## Real World Applications

This project can be used in:

- SMS filtering apps
- Email spam detection
- Banking fraud alerts
- Customer support systems
- Mobile messaging apps
- Telecom companies


## Future Enhancements

Possible improvements:

- Deep Learning (LSTM)
- Transformer models
- Web application deployment
- Flask/Django UI
- Real-time message API
- Email spam detection
- Multi-language spam classifier

## Conclusion

This project successfully classifies messages as spam or ham using Machine Learning.

By applying:

- NLP preprocessing
- TF-IDF vectorization
- Multinomial Naive Bayes

the system achieved strong performance.

This project demonstrates how Machine Learning can solve real-world text classification problems effectively.

---

## Developed By

Rithika Shanmugam

Final Year AIML
