Lab 4: Data Quality Assessment & Preprocessing (Housing Dataset)
Dataset Overview
The Housing.csv dataset contains 545 records with 13 attributes, covering property price, size, and key amenities such as parking, air conditioning, and furnishing status. This structure makes it suitable for predicting house prices and analyzing factors that influence value.

Preprocessing Summary
During preprocessing, I addressed three main issues: inconsistent feature scales (e.g., large price values vs. small count variables), the presence of outliers in price and area, and categorical features stored as text that needed numerical encoding. I also checked for missing values and prepared the data for modeling.

Missing Values
For simulated missing entries in the area column, I used median imputation. The median was selected because it is less sensitive to extreme property sizes and keeps the central tendency of the feature stable.

Outlier Handling
To reduce the impact of extreme prices, I applied the IQR method on the price column. After removing 15 outlier records, the dataset size decreased from 545 to 530 rows, resulting in a more reliable distribution for downstream models.

Feature Scaling
I applied Min–Max Scaling (0–1 range) and Z‑Score Normalization (mean 0, standard deviation 1) to the price and area features. This scaling step ensures that models which rely on distance or gradient-based optimization treat these features fairly.

Dimensionality Reduction (PCA)
Using PCA on six numerical features, I reduced the feature space while preserving most of the information. The first two principal components captured about 62.9% of the total variance, simplifying the data without losing its main patterns.

Objective
The goal of this lab was to clean, transform, and simplify the housing dataset so it is ready for machine learning tasks like regression or clustering. After preprocessing, the data is more consistent, less noisy, and better suited for building accurate and stable models.
