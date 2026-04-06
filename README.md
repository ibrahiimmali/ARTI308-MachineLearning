# Lab 6: Linear Regression Analysis - Ecommerce Customers

## Objective
This lab applies Linear Regression to an ecommerce dataset to study customer spending behavior. The main goal is to determine whether the Mobile App or the Website has a greater impact on Yearly Amount Spent.

## Dataset Overview
The dataset includes five main variables: Avg. Session Length, Time on App, Time on Website, Length of Membership, and Yearly Amount Spent. The first four are input features, while Yearly Amount Spent is the target variable.

## Tools Used
- Pandas and NumPy for data handling.
- Matplotlib and Seaborn for visualization.
- Scikit-Learn for model training and evaluation.

## Main Steps
- Performed exploratory data analysis using jointplots and pairplots.
- Split the data into training and testing sets.
- Trained a Linear Regression model.
- Evaluated the model using MAE, MSE, and RMSE.
- Plotted residuals to check model fit.

## Findings
The model showed that **Time on App** has a stronger effect on spending than **Time on Website**. The most important factor was **Length of Membership**, which had the highest positive relationship with Yearly Amount Spent.

## Conclusion
The results suggest that the company should focus more on improving the Mobile App and encouraging customer loyalty through longer membership.
