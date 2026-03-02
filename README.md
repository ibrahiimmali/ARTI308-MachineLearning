Lab 4: Data Quality Assessment & Preprocessing
Dataset Description
For this lab, I am using the Housing.csv Dataset, which consists of 545 rows and 13 features. This dataset includes critical property information such as price, area, and various amenities (e.g., air conditioning, furnishing status, and basement).

Preprocessing Findings
Data Quality Issues: Identified significant scale differences between features (e.g., price in millions vs. bedrooms in units), the presence of outliers, and categorical text data that requires numerical encoding.

Missing Value Strategy: Simulated and resolved missing data in the area column using Median Imputation. The median was chosen as it provides a robust center point that is not skewed by the extreme house sizes present in the data.

Outlier Management: Applied the Interquartile Range (IQR) method to the price column. By removing 15 extreme outliers, the dataset was stabilized from 545 to 530 rows for better model accuracy.

Normalization: Implemented both Min-Max Scaling (range 0–1) and Z-Score Normalization (mean 0, std 1) on the price and area columns to ensure features are on a comparable scale.

Dimension Reduction (PCA): Conducted Principal Component Analysis on six numerical features. The first two principal components captured 62.9% of the total dataset variance, successfully reducing complexity while retaining core information.

Goal
The objective of this lab was to clean, standardize, and reduce the dimensionality of the housing data. These preprocessing steps ensure the dataset is optimized for high-performance machine learning models, such as regression or clustering.
