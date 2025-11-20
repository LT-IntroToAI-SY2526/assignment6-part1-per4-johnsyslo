# Assignment 6 Part 1 - Writeup

**Name:** JP Syslo  
**Date:** 11/20/25

---

## Part 1: Understanding Your Model

### Question 1: R² Score Interpretation
What does the R² score tell you about your model? What does it mean if R² is close to 1? What if it's close to 0?

**YOUR ANSWER:**
The R^2 score tells me how much variation in test scores can be explained by the number of hours. If it's close to 1 the model fits the data and hours studied can be used as a strong predictor, if it's close to 0 it is a weak predictor.

---

### Question 2: Mean Squared Error (MSE)
What does the MSE (Mean Squared Error) mean in plain English? Why do you think we square the errors instead of just taking the average of the errors?

**YOUR ANSWER:**
MSE tells me how far off the model's predictions are from the actual test scores on avergae. The higher the MSE, the worse the model's accuracy. You squart the errors so that they all are positive, and it makes big mistakes hit harder than small ones --> helps the model learn.

---

### Question 3: Model Reliability
Would you trust this model to predict a score for a student who studied 10 hours? Why or why not? Consider:
- What's the maximum hours in your dataset?
- What happens when you make predictions outside the range of your training data?

**YOUR ANSWER:**
I would somewhat as the maximum of data is 9.8 hours but mainly stays in the 7-8 hour range. The linear regression can predict outside but the predictions are less reliable as it has not seen data in that range. 

---

## Part 2: Data Analysis

### Question 4: Relationship Description
Looking at your scatter plot, describe the relationship between hours studied and test scores. Is it:
- Strong or weak?
- Linear or non-linear?
- Positive or negative?

**YOUR ANSWER:**
From the scatter plot, the relationship between hours studied seems to be strong, linear, and positive. The only issue is around hours 8-9 where there is a clear difference in scores from hours studied.

---

### Question 5: Real-World Limitations
What are some real-world factors that could affect test scores that this model doesn't account for? List at least 3 factors.

**YOUR ANSWER:**
1. Amount of sleep before the test
2. A students motivation
3. Quality of studying/teaching or study materials


---

## Part 3: Code Reflection

### Question 6: Train/Test Split
Why do we split our data into training and testing sets? What would happen if we trained and tested on the same data?

**YOUR ANSWER:**
We split the data into training and testing sets so we can see how well the model preforms on data it has not seen. If we trained and tested on the same data, the model might look "perfect" but only because it memorized the training set. It would not generalize to new students or situations.

---

### Question 7: Most Challenging Part
What was the most challenging part of this assignment for you? How did you overcome it (or what help do you still need)?

**YOUR ANSWER:**
The most challenging part of the assignment was honestly the writeup and understanding how to use Anaconda and all of the imports. I had to learn and understand all of them in order to realize what the code was doing and answer the write up.

---

## Part 4: Extending Your Learning

### Question 8: Future Applications
Describe one real-world problem you could solve with linear regression. What would be your:
- **Feature (X):** 
- **Target (Y):** 
- **Why this relationship might be linear:**

**YOUR ANSWER:**
A real world problem that could use this is maybe the price of a used car based on milage.
- Feature (X): mileage
- Target (y): car price

As the mileage of the car goes up, the value of the car should decrease in a steady and predictable price.

---

## Grading Checklist (for your reference)

Before submitting, make sure you have:
- [x] Completed all functions in `a6_part1.py`
- [x] Generated and saved `scatter_plot.png`
- [x] Generated and saved `predictions_plot.png`
- [x] Answered all questions in this writeup with thoughtful responses
- [x] Pushed all files to GitHub (code, plots, and this writeup)

---

## Optional: Extra Credit (+2 points)

If you want to challenge yourself, modify your code to:
1. Try different train/test split ratios (60/40, 70/30, 90/10)
2. Record the R² score for each split
3. Explain below which split ratio worked best and why you think that is

**YOUR ANSWER:**
R^2 (60/40) => 0.9719
R^2 (70/30) => 0.9787
R^2 (90/10) => 0.9876

The 90/10 gave the highest R^2 score meaning the model explained almost all of the variance in the test scores for the split. The 90/10 split gives the model more training data and a tiny test set boosting R^2.