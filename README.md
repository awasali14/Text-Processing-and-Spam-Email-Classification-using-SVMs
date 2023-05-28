# Text-Processing-and-Spam-Email-Classification-using-SVMs

## Description

This repository contains code for a machine learning project that focuses on classifying emails as either spam or not spam. The project includes preprocessing steps, feature extraction, training a linear SVM model, and evaluating the model's performance. Additionally, the code provides a function to classify new email samples using the trained model.

## What was my motivation?

The motivation behind this project was to develop an effective and automated system for classifying emails as spam or not spam. This motivation stems from the need to help users filter out unwanted emails, reduce the risk of falling victim to scams or phishing attempts, and improve overall email management and security.

## Why did I build this project?

I built this project to tackle the problem of spam emails, which continue to be a significant issue for individuals and organizations. By building a machine learning model that can accurately classify emails, we can provide a practical solution to filter out unwanted emails and improve email user experience.

## What problem does it solve?

This project solves the problem of spam emails by leveraging machine learning techniques. It classifies emails as either spam or not spam, allowing users to focus on legitimate emails and reduce the time wasted on irrelevant or potentially harmful messages. By automating the classification process, it enhances email management and security.

## What did I learn?

Throughout the project, I learned several key concepts and techniques, including:

Text preprocessing: I gained experience in preprocessing textual data by converting text to lowercase, removing HTML tags, replacing special characters, and performing tokenization.

Feature extraction: I learned how to extract meaningful features from text data using a vocabulary list and binary feature vectors to represent the presence or absence of words.

Machine learning model training: I gained knowledge in training a linear SVM model using labeled training data and optimizing hyperparameters to improve model performance.

Model evaluation: I learned how to evaluate the accuracy of a trained model on both the training and test datasets to assess its performance.

Application development: I acquired skills in developing a practical application that can classify new email samples using the trained model.


## Features

Preprocessing of email content: The code reads the content of an email file, converts it to lowercase, removes HTML tags, replaces special characters, and performs word tokenization.
Vocabulary extraction: The code reads a vocabulary file and extracts the vocabulary list to be used as features for email classification.
Feature extraction: The code checks the presence of each vocabulary word in the processed email content and creates a binary feature vector indicating the occurrence of each word.
Training of a linear SVM model: The code trains a linear SVM model using the extracted features and corresponding labels from a labeled training dataset.
Evaluation of model performance: The code evaluates the trained model's accuracy on both the training and test datasets.
Classification of new email samples: The code provides a function to classify new email samples using the trained model and the same preprocessing and feature extraction steps.

## Usage

To use the code, follow these steps:

Clone the repository

Set up the dataset:

Prepare the training dataset: Download the spamTrain.mat file containing labeled spam and non-spam emails and place it in the appropriate directory within the project structure.
Prepare the test dataset: Download the spamTest.mat file for evaluating the trained model and place it in the appropriate directory within the project structure.

Set up the email sample:

Prepare the email sample: Create an email file or use an existing one that you want to classify. Update the file variable in the code to specify the path to the email file.
Execute the code:

Run the script to perform email classification and display the results.

## Results

After running the code, the following results will be displayed:

Training Accuracy: The accuracy of the trained model on the training dataset, expressed as a percentage.

Test Accuracy: The accuracy of the trained model on the test dataset, expressed as a percentage.

Additionally, the code will classify a provided email sample as either spam or not spam.

## Preprocess Function

The code includes a preprocess function that performs the following preprocessing steps on the email content:

Read the contents of the email file.
Convert the contents to lowercase.
Remove HTML tags by erasing text between < and > characters.
Replace the $ symbol with the word "dollar".
Split the processed content into individual words.
Replace URLs starting with "http://" or "https://" with the word "httpaddr".
Replace email addresses with the word "emailaddr".
Replace numeric strings with the word "number".
Remove non-alphanumeric characters.
Remove words with a length less than or equal to 1.
Apply stemming to each word using the Porter stemming algorithm.

## Conclusion

Overall, this project provided hands-on experience in tackling a real-world problem using machine learning techniques, while also enhancing my understanding of text preprocessing, feature extraction, model training, and evaluation.
