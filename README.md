
# Netflix Reviews Sentiment Analysis

This project focuses on performing sentiment analysis on Netflix reviews from the App Store. The reviews vary widely, ranging from highly positive feedback to very negative comments. The goal of this project is to classify these reviews into two distinct categories: positive and negative.


# Project Overview

By leveraging natural language processing (NLP) techniques and machine learning algorithms - LSTM, we aim to analyze the sentiments expressed in the reviews. This classification will help us better understand the overall customer satisfaction and identify common themes in both positive and negative feedback.








## Data Background
The dataset to train the model is from Kaggle
[DATASET](https://www.kaggle.com/code/darrylljk/analysis-netflix-reviews-with-nlp/input)

The dataset has one csv file that has ID, Name, Content, Score, App Version





## Run Locally

To run this project locally, ensure you have the following libraries installed:

```bash
  pip install pandas
  pip install numpy
  pip install scikit-learn
  pip install nltk
  pip install tensorflow

```
    
## Structure of the project


### Data Cleaning
- Check and handle Null values, the content column had few NaN values which was removed

### Data Pre-processing
- Take necessary columns - content and score
- Make a new column ["sentiment"] and set it to 1 if score is 3,4,5 and 0 if score is 1,2
- Use porterstemmer and make a corpus of each review.
- Use tokenizer to convert the text into sequences.
- Make all arrays to an equal size

### Model Training
- Generate train and test dataset to feed into the Sequential Model
- Add necessary layers to create the LSTM model.
- Fit the model on training dataset and calculate accuracy


### Performance
- The accuracy is 0.8591 

### Check with Input
- Use custom input and check to see how classification works.
## ER Diagram

![ER Diagram](https://github.com/KiranSeetharam11/Cheque-Details-Recognition/blob/main/Cheque%20ER.png)

