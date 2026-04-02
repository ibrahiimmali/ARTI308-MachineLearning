# Lab 4: Data Quality Assessment & Preprocessing

## Dataset Description
The `Housing.csv` dataset contains **545** rows and **13** features, including price, area, and amenities such as air conditioning, basement, parking, and furnishing status. It is suitable for house price prediction and understanding which property characteristics affect value.

## Preprocessing Findings
I observed scale differences between features (price vs. count variables), outliers in key numeric columns, and categorical attributes stored as text that required numerical encoding. I also checked for missing values and prepared the data for later modeling steps.

## Missing Values
For simulated missing values in the `area` column, I used **median imputation**. The median is more robust than the mean in this dataset because some houses have extremely large areas that would skew the average.

## Outlier Management
I applied the **Interquartile Range (IQR)** method to the `price` column to detect and remove extreme outliers. After dropping **15** outlier records, the dataset size went from **545** to **530** rows, giving a more stable price distribution.

## Normalization
To put features on a comparable scale, I applied **Min–Max Scaling** (range 0–1) and **Z‑Score Normalization** (mean 0, standard deviation 1) to the `price` and `area` columns. This helps distance‑based and gradient‑based models train more effectively.

## Dimensionality Reduction (PCA)
I ran **Principal Component Analysis (PCA)** on six numerical features. The first two principal components captured about **62.9%** of the total variance, reducing dimensionality while preserving most of the important information.

## Goal
The goal of this lab was to clean, scale, and simplify the housing data to make it ready for machine learning tasks like regression or clustering. After preprocessing, the dataset is more consistent, less noisy, and better suited for building accurate models.
