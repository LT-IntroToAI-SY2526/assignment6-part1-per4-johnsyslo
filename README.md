---
title: 'Assignment 6 Part 1: Introduction to Data & Linear Regression'
author: 'Mr. Berg, Lane Tech College Prep'
geometry: margin=1in
---

# Setup Instructions - IMPORTANT!

For this unit, we'll be using data science libraries that require a special Python environment. Follow these steps:

1. **Open Anaconda Navigator** on your computer
2. **Wait for it to fully load** (this can take a minute or two)
3. **Click on VS Code** from within Anaconda Navigator
4. **Open this assignment folder** in VS Code

**Why?** Anaconda provides a virtual environment with all the data science libraries (numpy, pandas, sklearn, matplotlib) pre-installed. If you open VS Code directly without going through Anaconda, these libraries won't be available.

**Troubleshooting:**
- If you get a "ModuleNotFoundError", you probably didn't open VS Code through Anaconda
- Close VS Code completely and reopen it through Anaconda Navigator

---

# Assignment Overview

In this assignment, you'll learn the fundamentals of **linear regression** - a machine learning technique that finds relationships between variables and makes predictions. 

## What You'll Learn

1. **Loading and exploring data** with pandas
2. **Visualizing relationships** with matplotlib
3. **Building a simple linear regression model** with sklearn
4. **Splitting data** into training and testing sets
5. **Evaluating model performance** with metrics

## Real-World Applications

Linear regression is everywhere:
- **Real estate:** Predicting house prices based on square footage
- **Business:** Forecasting sales based on advertising spend
- **Medicine:** Predicting patient outcomes based on health metrics
- **Sports:** Estimating player performance based on training data

---

# Part 1: In-Class Example - Ice Cream Sales

We'll walk through a complete example together in class using `ice_cream_example.py`. This example predicts ice cream sales based on temperature.

**What we'll cover:**
- Loading data from a CSV file
- Creating scatter plots to visualize relationships
- Training a linear regression model
- Making predictions
- Understanding metrics (R² score, MSE)

---

# Part 2: Your Assignment - Student Performance

After the in-class example, you'll complete `a6_part1.py` which predicts student test scores based on hours studied.

## Dataset

You'll work with `student_scores.csv` which contains:
- **Hours**: Number of hours a student studied
- **Scores**: Test score the student received

## Your Tasks

Complete the following functions in `a6_part1.py`:

1. **`load_and_explore_data(filename)`**
   - Load the CSV file
   - Print basic statistics (mean, min, max)
   - Return the dataframe

2. **`create_scatter_plot(data)`**
   - Create a scatter plot of Hours vs Scores
   - Add labels and title
   - Save the plot

3. **`split_data(data)`**
   - Split into features (X) and target (y)
   - Split into training (80%) and testing (20%) sets
   - Return X_train, X_test, y_train, y_test

4. **`train_model(X_train, y_train)`**
   - Create and train a LinearRegression model
   - Return the trained model

5. **`evaluate_model(model, X_test, y_test)`**
   - Make predictions on test data
   - Calculate and print R² score and MSE
   - Return predictions

6. **`visualize_results(X_test, y_test, predictions)`**
   - Plot actual vs predicted values
   - Add a line of best fit
   - Save the visualization

## Deliverables

1. **Completed `a6_part1.py`** with all functions implemented
2. **Two saved plots:**
   - `scatter_plot.png` - original data
   - `predictions_plot.png` - model results
3. **Completed `a6_part1_writeup.md`** with thoughtful answers to all reflection questions

---

# Grading Rubric (10 points)

- **Code Functionality (4 points)**
  - All functions work correctly
  - Code follows good practices (variable names, comments)
  
- **Visualizations (2 points)**
  - Both plots are clear and properly labeled
  - Saved with correct filenames

- **Writeup (4 points)**
  - All questions answered with thoughtful, complete responses
  - Demonstrates understanding of R², MSE, and model limitations
  - Shows critical thinking about real-world applications

---

# Helpful Resources

- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)
- [Sklearn Linear Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)
- [Understanding R² Score](https://statisticsbyjim.com/regression/interpret-r-squared-regression/)

---

# Due Date

This assignment is due **[INSERT DATE]**. Push your completed code to GitHub and make sure your plots are committed as well.

**Questions?** Ask in class or come to office hours!
