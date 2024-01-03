# Handwritten-Digit-Recognition

MNIST Digit Recognition Project

This project is a simple implementation of digit recognition using the MNIST dataset. The goal is to train a logistic regression classifier to identify whether a given digit is the number '2' or not.

The project focuses on utilizing the MNIST dataset, a collection of 28x28 pixel grayscale images of handwritten digits (0 through 9). The specific objective is to create a logistic regression model capable of identifying whether a given digit is the number '2' or not.

Installation
Ensure you have the required dependencies installed. You can install them using the following:

Usage

Clone the repository and run the Jupyter notebook provided in the project. The notebook (mnist_digit_recognition.ipynb) contains the entire code along with explanations for each step.

Dataset

The MNIST dataset is fetched using the fetch_openml function from scikit-learn. It contains both the pixel data (x) and the corresponding labels (y).

Libraries Used


NumPy: For numerical operations and array handling.

Pandas: For data manipulation and analysis.

Scikit-learn: Used for machine learning tasks, including dataset fetching, model training, and evaluation.

Matplotlib: For data visualization.

Fetching Dataset

The MNIST dataset is fetched using the fetch_openml function.

Data Exploration

The dataset is explored to understand its structure, including the shape of the input features (x) and labels (y).

Data Preprocessing

Data preprocessing involves shuffling the data and converting labels to a binary format suitable for a binary classification task.

Model Training

A logistic regression model is trained using the LogisticRegression class from scikit-learn.

Model Evaluation

Model performance is evaluated using cross-validation to obtain an accuracy score.

Warnings

Index Issue: There is a check for the existence of a specific index (36000) in the DataFrame. Ensure the index is present to avoid errors.
Deprecation Warning: The tol parameter in LogisticRegression is set to 0.1 to avoid convergence warnings. Adjust it as needed.
