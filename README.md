# Sentiment-analysis using Deep Learning

## Project Overview
This project implements a sentiment analysis model using deep learning techniques. The model is trained to classify text into three sentiment categories: Negative, Neutral, and Positive. It leverages tokenization, padding, and embedding layers to process text data and a neural network for classification.

## Dataset
The dataset consists of labeled text samples with sentiment categories:
> Negative (0)
> Neutral (1)
> Positive (2)
Class distribution was analyzed and stratified splitting was applied to maintain balance during training and testing.

## Preprocessing Steps
> Text Cleaning - Removal of punctuation, special characters, and converting text to lowercase.
> Stopword Removal & Lemmatization - Helps in reducing noise and standardizing text.
> Tokenization & Padding - Converts text into numerical sequences suitable for model input.
> Handling Negations - Specific negation words were retained to maintain sentiment context.

## Training
> The dataset was split into 80% training and 20% testing.
> The model was trained for 5 epochs using a batch size of 64.
> The optimizer used was Adam, with categorical cross-entropy loss.
> Accuracy and loss were monitored for both training and validation sets.

## Performance & Findings
> Training Accuracy improved steadily, reaching ~91%.
> Validation Accuracy peaked at ~72%, but validation loss increased, indicating overfitting.
> Possible improvements include regularization techniques (dropout, L2 regularization) and data augmentation.

## Prediction & User Input Testing
A function was implemented to allow user input testing, where a user enters a text, and the model predicts its sentiment. The output is displayed in human-readable labels instead of numerical class values.

## Author
This project was collaboratively developed with a focus on machine learning and NLP techniques.

