
# Linear Regression from Scratch in Python

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Prerequisites](#prerequisites)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Dataset](#dataset)
7. [Code Explanation](#code-explanation)
    - [1. Data Preprocessing](#1-data-preprocessing)
    - [2. Model Implementation](#2-model-implementation)
    - [3. Model Training](#3-model-training)
    - [4. Model Evaluation](#4-model-evaluation)
    - [5. Visualization](#5-visualization)
8. [Results](#results)
9. [Contributing](#contributing)
10. [License](#license)

---

## Introduction
This project demonstrates the implementation of **Simple Linear Regression** from scratch using Python and **NumPy** without relying on machine learning libraries like Scikit-Learn. The model predicts house prices based on various features like house size, number of bedrooms, and age of the house.

## Features
- Implementation of linear regression using **Normal Equation**.
- Data preprocessing with normalization and handling missing values.
- Evaluation metrics: **Mean Squared Error (MSE)** for both training and testing sets.
- Visualization of results.

## Prerequisites
To run this project, you need the following:
- Python 3.x
- NumPy
- Pandas
- Matplotlib

## Installation
Clone this repository to your local machine:
\`\`\`bash
git clone https://github.com/your-username/linear-regression-from-scratch.git
\`\`\`

Install the required packages:
\`\`\`bash
pip install numpy pandas matplotlib
\`\`\`

## Usage
1. Ensure that the dataset (house_prices.csv) is placed in the project directory.
2. Run the Python script to train the model and evaluate it:
   \`\`\`bash
   python linear_regression.py
   \`\`\`
3. The output will display the Mean Squared Error for both the training and testing sets, along with a plot visualizing the model's predictions.

## Dataset
The dataset used for this project is `datasets_house_prices.csv`, which includes features like:
- `Size`: Size of the house in square feet.
- `Bedrooms`: Number of bedrooms.
- `Age`: Age of the house.
- `Price`: Target variable representing the price of the house.

## Code Explanation

### 1. Data Preprocessing
- Load the dataset using **Pandas**.
- Fill any missing values with the mean.
- Normalize the feature columns (`Size`, `Bedrooms`, `Age`) for better model performance.

### 2. Model Implementation
- A `LinearRegression` class is defined.
- The `fit` method uses the **Normal Equation** to compute the model parameters.
- The `predict` method generates predictions using the trained model.

### 3. Model Training
- Data is split into training and testing sets (80% training, 20% testing).
- The linear regression model is trained on the training set.

### 4. Model Evaluation
- The model is evaluated using **Mean Squared Error (MSE)** on both the training and testing sets to measure its performance.

### 5. Visualization
- A scatter plot is generated to visualize the relationship between house size and price, comparing actual prices with the predicted ones.

## Results
- The Mean Squared Error (MSE) for the training and testing sets will be displayed in the console.
- A plot visualizing the model’s predictions versus actual data for house size and price is generated.

## Contributing
Contributions are welcome! If you'd like to add new features or improve the current implementation, please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature (`git checkout -b feature-name`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push the branch (`git push origin feature-name`).
5. Create a new Pull Request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
