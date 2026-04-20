# K Nearest Neighbors Project

## Objective
This project uses the K-Nearest Neighbors (KNN) algorithm to classify whether a customer belongs to the target class based on several numerical features. The goal is to build a model that can predict the class using distance-based pattern recognition.

## Dataset Overview
The dataset contains 10 feature columns and one target column, `TARGET CLASS`. The features include variables such as XVPM, GWYH, TRAT, and others, which represent numerical customer data used for classification.

## Tools Used
- Pandas and NumPy for data handling.
- Matplotlib and Seaborn for visualization.
- Scikit-Learn for scaling, train-test splitting, and KNN classification.

## Main Steps
- Loaded and explored the dataset.
- Standardized the feature values.
- Split the data into training and testing sets.
- Trained a KNN model.
- Evaluated model performance using predictions and error checks.

## Conclusion
This lab shows how KNN can be used to classify data based on similarity between observations. Feature scaling is important because KNN depends on distance calculations.
