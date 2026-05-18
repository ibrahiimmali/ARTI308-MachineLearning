# Credit Card Customer Segmentation Project - Lab11

## Objective
This project uses K-Means clustering to segment credit card customers based on their spending and usage behavior. Since there is no target label, the goal is to discover natural customer groups in the data.

## Dataset Overview
The dataset contains customer-level credit card activity features such as balance, purchases, cash advance, credit limit, payments, and tenure. Each row represents one customer, and the data is used for unsupervised learning.

## Tools Used
- Pandas and NumPy for data handling.
- Matplotlib and Seaborn for visualization.
- Scikit-Learn for scaling, clustering, PCA, and evaluation.

## Main Steps
- Loaded and inspected the dataset.
- Checked missing values and summary statistics.
- Scaled the features using StandardScaler.
- Applied K-Means clustering.
- Used PCA to visualize the clusters.
- Reviewed cluster counts and cluster characteristics.

## Conclusion
This lab shows how clustering can be used to group similar customers and support better business decisions, such as targeted marketing and customer segmentation.
